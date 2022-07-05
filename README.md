# GVol Python Tutorial

These notebooks are intended to help you learn Python, get up to speed on basic programming concept and finally building your own options analytics code using the GVol Python module.

## Lesson 1: Installation, Variables and Functions - Resources

[Lesson 1 Python Code](https://github.com/genesis-volatility/python-tutorial/blob/master/GVol%20%3C%3E%20Python%20Part%201%20-%20Variables%20and%20Functions.ipynb)

[Lesson 1 Youtube Tutorial](https://youtu.be/X0Pzw8jTiFM)

[Install Python on Mac OS](https://docs.python-guide.org/starting/install3/osx/)

[Install Python on Windows](https://www.python.org/)

[Additional Resources on functions and variables](https://www.w3schools.com/python/python_functions.asp)

## Lesson 2: Using Pandas - Resources

[Lesson 2 Python Code](https://github.com/genesis-volatility/python-tutorial/blob/master/GVol%20%3C%3E%20Python%20Part%202%20-%20Pandas.ipynb)

[Lesson 2 Youtube Tutorial](https://youtu.be/GkYFpGNxl_Y)

[Pandas Documentation](https://docs.python-guide.org/starting/install3/osx/)

[Numpy Documentation](https://numpy.org/doc/)

## Lesson 3: Installation, Variables and Functions - Resources

[Lesson 3 Python Code](https://github.com/genesis-volatility/python-tutorial/blob/master/GVol%20%3C%3E%20Python%20Part%203%20-%20Plotly.ipynb)

[Lesson 3 Youtube Tutorial](https://youtu.be/LqkLYd1xszM)

[Using Plotly with Pandas](https://docs.python-guide.org/starting/install3/osx/)

[Plotly Documentation](https://plotly.com/python/getting-started/)

## Lesson 4:

[Lesson 4 Python Code](https://github.com/genesis-volatility/python-tutorial/blob/master/GVol%20%3C%3E%20Python%20Part%204%20-%20GVol%20Module.ipynb)

[Lesson 4 Youtube Tutorial](https://youtu.be/2QTTF0gSRyg)

[GVol API-Lite Documentation](https://docs-lite.gvol.io/)

[GVol Pro Documentation](https://docs.gvol.io/)

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [gvol](https://pypi.org/project/gvol/).

```bash
pip install gvol
```

Basic GVol usage.

```python
from gvol import GVol

#create GVol Client
gvol_client = GVol(header='x-oracle',gvol_api_key=GVOL_API_KEY)
gvol_client = GVol(header='gvol-lite-plus',gvol_api_key=GVOL_API_KEY_LITE_PLUS)
gvol_client = GVol(header='gvol-lite',gvol_api_key=GVOL_API_KEY_LITE)

##SELECT EXCHANGE: (Supported exchanges are |deribit|bitcom|okex|delta|)
exchange = 'deribit'

data = gvol_client.options_orderbook_details(exchange=exchange)

```

### Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Find Edge, Capture Alpha, Slang Size.
:heart: [gvol.io](www.gvol.io) :heart:
info@genesisvolatility.io
