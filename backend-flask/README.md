'''docker run --rm -p 4566:4567 -it -e FRONTEND_URL="*" -e BACKEND_URL="*" backend-flask'''

# Install python version
```
pyenv install 3.10.9
```

# Set your python version
```
pyenv global 3.10.9
```

# Create virual environment
```
python -m venv venv
```

# Activate environment
```
source venv/bin/activate
```

# Install Flask
```
pip install flask
```

# Build Docker container
'''
docker build -t backend-flask ./backend-flask
'''

# Run Container
'''
docker run --rm -p 4567:4567 -it backend-flask
'''