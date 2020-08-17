# Notes from Udemy course
## MetaMask seed backup phrase: 
    move absent broken 
    cupboard tide fabric 
    few ecology wish 
    town alert balcony

## Section 2 (8/15/20 - 8/16/20)

### 42. Testing with Mocha
- Deleted simple mocha test example which was inside './test/Inbox.test.js'

```js
class Car {
    park() {
        return 'stopped';
    }

    drive() {
        return 'vroom';
    }
}

let car;

beforeEach( () => {
    car = new Car();
});

describe('Car', () => {

    it('can park', () => {
        assert.equal(car.park(), 'stopped');
    });

    it('can drive', () => {
        assert.equal(car.drive(), 'vroom');
    });
})
```

### 45. Refactor to Async/Await
- Before refactoring beforeEach()

```js
beforeEach(() => {
    // Get a list of all acounts
    web3.eth.getAccounts() // this function returns a promise
        .then(fetchedAccounts => {
            console.log(fetchedAccounts);
        });

});
```