# Axios Read Me

1. Install
```
npm install axios
```

2. import axios
```
import axios from 'axios';
```

3. Get request / fetch from an api
```
axios.get('https://pokeapi.co/api/v2/pokemon?limit=807')
    .then(response => {
        setPokemonList(response.data.results)
    })
    .catch(err -> console.lof("Error"))
```