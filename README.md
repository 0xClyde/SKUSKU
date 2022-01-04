
# The Directory

The directory is a truffle project that contains the required
contract, migration and test files.


### State variables

    The contract have an owner, of type address that is public.
   

    </details>

  - [ ] should have an skuCount
    <details><summary>:book:</summary>

    The contract will keep track of the [sku](https://en.wikipedia.org/wiki/Stock_keeping_unit)s in our supply
    chain. Each item for sale will have a unique sku number. 



    </details>

### enum State

Items can exist in our Supply chain domain in a few states. In Solidity an
`enum` can be used to represent these different states. Remove the `skip`
annotation from the enum tests to proceed.

  - [ ] `ForSale` for when an item is put on sale
  - [ ] `Sold` for when an item has been purchased
  - [ ] `Shipped` for when an item has been shippd to the buyer
  - [ ] `Received` for when the shipped item has been received by the buyer

### Item struct

How do we describe an item in our supply chain? It is a union of properties:
`name`, `sku`, `price`, `state`, `seller` and `buyer`. We can use a Solidity
`struct` to model this Item.



