# cardtest

Open Source framework for distributed testing of smart cards on multiple cards / card readers on multiple nodes with support for hot-swapping of cards, readers and nodes.

## Design

The cardtest framework should be independent of the actual framework or library used to access the smart card readers.
The default would be `javax.smartcardio`.

In order to be able to test with `javax.smartcardio` without actually having a nodes and readers, a fake implementation of `javax.smartcardio` will be useful.
Whether this fake implementation should be in this project or another project is yet to be decided.
