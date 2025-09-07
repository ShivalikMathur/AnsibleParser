Project Overview:
This project serves as a hands-on exploration of metaprogramming concepts and Domain-Specific Language (DSL) implementation through the creation of a specialized Ansible inventory parser. The core objective was to develop a comprehensive parsing system that performs both lexical analysis and syntactic parsing of Ansible inventory files, with the specific goal of identifying and enumerating all host definitions within these infrastructure configuration files. This practical implementation provides valuable insights into how infrastructure-as-code tools like Ansible process and interpret their declarative configuration inputs.

Project Components:
The implementation consists of four key components:

lexer.l - Contains the Flex lexical analyzer specification that defines tokenization rules for processing Ansible inventory files. This component breaks down the input text into meaningful tokens such as keywords, hostnames, and various identifiers.

parser.y - Houses the Bison parser generator definitions that establish the grammatical structure and syntax rules for Ansible inventory files. The parser includes embedded actions that trigger specific behaviors, such as incrementing host and group counters, when particular syntactic patterns are encountered during parsing.

inventory - Serves as a representative sample of an Ansible inventory file, demonstrating the expected format and structure that the parsing system is engineered to process effectively.

test.sh - Provides an automated testing framework to validate the parser's functionality and ensure reliable operation across different inventory file configurations.
