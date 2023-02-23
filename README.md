# Genetic Algorithm-based attack on the vigenère cipher
The file above contains the code of a genetic algorithm based attack that manages to break polymorphic substitution ciphers

# Process
The keys, in a vigenère cipher, are strings that need to be encoded to integers within the range of alphabets (0..25). Tournament selection, where parent chromosomes within the population are selected randomly for mating, is used in this specific case along with the roulette wheel selection. Then, a  crossover will occur to the parents that had been selected. During this study, the crossover types used are single-point and two-points crossovers and they work by randomly selecting points where the crossover will occur to generate different encryption keys. According to a certain rate that is correlated with the key length, some chromosomes will be mutated to maintain diversity within the population and avoid premature convergence. The random mutation type, which is used during this study, will randomly mutate genes within some chromosomes. Then, the new population will be evaluated using the fitness function; each encryption key will be associated with a score that could be an n-grams score or the number of correct letters found while decrypting the ciphertext using the relevant chromosome (key). 

### CopyRights 
Louai Zaiter