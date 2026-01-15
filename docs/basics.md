
# 🧠 Conceptos Básicos

## Tocar notas

```python
play 60
play :C4
```

## Silencios

```python
play :C4
sleep 1
play :E4
sleep 0.5
play :G4
```

## Loop

```python
loop do
  play :C2
  sleep 1
end
```