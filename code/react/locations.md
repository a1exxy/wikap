# React - Использоание url

## Текущей путь
```
  const currentLocation = useLocation().pathname
```

## Параметры в URL (те что после '?')
```
  const search = useLocation().search;
  const filter = new URLSearchParams(search).get('filter');
```
