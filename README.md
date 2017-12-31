# couscous-python
Docker image based on composer, adding couscous, python

## Usage

```
docker run -it --rm -p $PORT:8000 -v "$YOUR_COUSCOUS_PATH":/project \
	yuwash/couscous-python preview 0.0.0.0:8000
```
