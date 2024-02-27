# Fiestal-Cipher
All Codes of Fiestal Cipher.
Constants and S-boxes: Defines the expansion permutation table, S-boxes, and P-box transposition table.

generate_round_key(): Generates a random 48-bit round key.

expand_to_48_bits(right_half): Expands the 32-bit right half of the input block to 48 bits using the expansion permutation table.

substitute_with_s_boxes(expanded_half): Performs S-box substitution by dividing the 48-bit block into segments and substituting each segment using the corresponding S-box.

transposition_p_box(output): Applies a fixed permutation to the output bits using the P-box transposition table.

single_round_des(right_half, round_key): Encapsulates a single round of DES encryption, including expansion, substitution, transposition, and XOR operations with the round key.

Example usage: Generates a random 32-bit right half of the input block and a random 48-bit round key, then performs one round of DES encryption and prints the result.
