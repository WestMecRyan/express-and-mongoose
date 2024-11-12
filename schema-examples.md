# Tour Web Site Model

```js
const tourSchema = new mongoose.Schema({
    name: {
        type: String,
        required: [true, 'A tour must have a name']
    },
    rating: {
        type: number,
        default: 4.5
    },
    price: {
        type: number,
        required: [true, 'A tour must have a price'];
    }
});

const Tour = mongoose.model('Tour', tourSchema);
```