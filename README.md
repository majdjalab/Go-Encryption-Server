# Encryption Web Application

This is a web application built in Go that provides text encryption and decryption functionality using the AES (Advanced Encryption Standard) algorithm. The app allows users to securely encrypt and decrypt sensitive information, such as names and addresses, through a simple web interface.

## Features

- **AES Encryption and Decryption**: Encrypt and decrypt text using the AES algorithm with a predefined secret key.
- **Base64 Encoding/Decoding**: Encode encrypted data in Base64 format for easy storage and transmission.
- **Simple Web Interface**: Easy-to-use HTML form to input text for encryption/decryption.
- **Error Handling**: Robust error handling to ensure reliability and security.
- **Ready to Deploy**: Can be easily deployed to any web server supporting Go applications.

## Prerequisites

- Go 1.16 or later installed on your system.
- A web browser to access the front-end form.

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/majdjalab/go-encryption-server.git
    cd go-encryption-server
    ```

2. **Build the application**:

    ```bash
    go build -o encryption-app
    ```

3. **Run the application**:

    ```bash
    ./encryption-app
    ```

4. **Access the application**:

   Open your web browser and navigate to `http://localhost:[Your Port]` to access the encryption form.

## Usage

- **Encrypt Text**: Enter the text you want to encrypt in the input form, then submit the form. The encrypted result will be displayed on the page.
- **Decrypt Text**: Paste the Base64-encoded encrypted text into the input form and submit to decrypt it back to plain text.

## Configuration

- **Modify the Secret Key**: The encryption key (`MySecret`) is currently hardcoded in the source code for simplicity. For production use, it is recommended to store this key securely, such as in an environment variable or a secure vault.
- **Adjust the Initialization Vector (IV)**: The IV is also hardcoded. You can modify this to use a dynamically generated IV for each encryption operation to enhance security.

## Security Considerations

- **HTTPS**: Deploy the application behind an HTTPS server to ensure secure transmission of sensitive data.
- **Dynamic IV**: Consider using a random IV for each encryption operation instead of a fixed one.
- **Environment Variables**: Store secrets like encryption keys in environment variables or a secure secrets manager instead of hardcoding them.

## Contributing

Contributions are welcome! Feel free to submit issues and pull requests.

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature-branch`)
6. Open a pull request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Go Programming Language](https://golang.org/)
- [AES Encryption Algorithm](https://en.wikipedia.org/wiki/Advanced_Encryption_Standard)

## Contact

If you have any questions or suggestions, please open an issue or contact me at [majdjalab@gmail.com].

---

Happy Encrypting!
