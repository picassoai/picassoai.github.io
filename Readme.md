# Adding New Acuators
1. Add an image of the actuator (preferably 700x700) to `assets/img/products/`
2. Create a .json file in `assets/specdata/`
3. Add the json file name to `assets/specdata/fileList.txt`

### JSON schema
The json file must have the following attributes:
   - `title (string)`: name of the actuator
   - `price (number)`: price of the actuator
   - `stock (number)`: amount of the actuator in inventory
   - `description (string)`: description of actuator shown on the actuator's own product page
   - `blurb (string)`: short description of actuator shown on products.html'
   - `image (string)`: link to image in the `assets/img/products/` directory
   - `specifications (list)`: list of actuator attributes to be displayed on the products page

### Example JSON
```
{
    "title": "AK10-9 V2",
    "price": 500,
    "stock": 300,
    "description": "The AK10-9 V2 is a cost-effective, high performance actuator that ...",
    "blurb": "Operating temp: -20°C~50°C<br>Voltage: 24/48 V<br>14bit high resolution magnetic encoder<br>",
    "image": "assets/img/products/AK10-9 V2.jpg",
    "specifications": {
        "Operating temp": "-20°C~50°C",
        "Phase": "Three Phase",
        "Reduction ratio": "10:1",
        "Back drive (Nm)": "0.48",
        "Rated voltage (V)": "24/48",
        "Rated torque (Nm)": "0.83",
    }
}
```