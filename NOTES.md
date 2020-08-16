# Notes from Udemy course ()

## Section 2 (8/15/20)

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