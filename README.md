# HTTP Server in Rust  

## _A Simple, Educational HTTP Server_  

[![Rust](https://img.shields.io/badge/Rust-1.65%2B-orange)](https://www.rust-lang.org/)  
[![Build Status](https://travis-ci.org/sahilmadaan048/http-server.svg?branch=main)](https://travis-ci.org/sahilmadaan048/http-server)  

This project is a basic HTTP server implemented in Rust. It serves as an educational tool to understand how the web works and lays the foundation for creating a multi-threaded web framework in Rust.  

## Features  

- ✅ Implements a simple HTTP server.  
- ✅ Supports basic HTTP methods: `GET`, `POST`, `PUT`, and `DELETE`.  
- ✅ Parses incoming HTTP requests and extracts headers and body data.  
- ✅ Uses `TcpListener` to accept incoming connections.  
- ✅ Utilizes `BufReader` for efficient stream handling.  
- ✅ Demonstrates fundamental networking concepts in Rust.  

## Tech Stack  

This project is built with:  

- 🦀 [Rust](https://www.rust-lang.org/) – Safe and performant systems programming.  
- 📡 [Tokio](https://tokio.rs/) – Async runtime for networking in Rust.  
- 🌐 [Hyper](https://hyper.rs/) (Future Integration) – HTTP library for Rust.  

## Installation  

Ensure you have Rust installed. If not, install it using [rustup](https://rustup.rs/):  

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Clone the repository:  

```sh
git clone https://github.com/sahilmadaan048/http-server.git
cd http-server
```

Build and run the server:  

```sh
cargo run
```

By default, the server listens on `0.0.0.0:8080`.  

## Code Structure  

| Component | Description |  
| --------- | ----------- |  
| `Server` | Represents the host that listens for incoming connections. |  
| `Client` | Represents the end-user making requests. |  
| `Request` | Handles incoming HTTP requests by parsing method, headers, and body. |  
| `Response` | _(Planned)_ Handles server responses. |  
| `read_header_line()` | Reads HTTP headers from the TCP stream. |  
| `main()` | Initializes the server and processes incoming requests. |  

## Future Improvements  

- 🔹 Implement proper HTTP response handling.  
- 🔹 Add multi-threaded request processing.  
- 🔹 Improve error handling and logging.  
- 🔹 Enhance request parsing to handle more HTTP features.  

## Contributing  

Want to contribute? Great!  

1. Fork the repository.  
2. Create a feature branch (`git checkout -b feature-branch`).  
3. Commit your changes (`git commit -m "Add a new feature"`).  
4. Push to the branch (`git push origin feature-branch`).  
5. Open a Pull Request.  

## License  

MIT License.  

🚀 **Free Software, Hell Yeah!**  

For full source code, visit: [GitHub Repository](https://github.com/sahilmadaan048/http-server.git)  
