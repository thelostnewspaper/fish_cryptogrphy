# fish_cryptogrphy

In this project, we developed an interactive cryptographic tool that utilizes randomness extracted from video frames to generate secure cryptographic keys. The process involved several key steps:

Video Processing: We used OpenCV to read frames from a video file. Each frame was converted to greyscale and then to a binary format, allowing us to extract randomness from the pixel data.

Combining Randomness: The binary data from all processed frames was combined into a single array, providing a rich source of entropy for key generation.

Key Derivation: We implemented the PBKDF2 (Password-Based Key Derivation Function 2) algorithm to derive a cryptographic key from a user-provided password. This process included generating a random salt to enhance security.

Interactive Encryption and Decryption: The tool engaged users by prompting them to enter a password for key generation. After generating the key, users were asked if they wanted to proceed with encrypting a plaintext message. If they agreed, the message was encrypted using AES (Advanced Encryption Standard). The user was then given the option to decrypt the ciphertext, allowing them to see the original message.

This project effectively combined video processing, cryptographic key generation, and user interaction, demonstrating the practical application of cryptographic principles while making the process accessible and informative for users.
