

# 🎹 Melodía y Sintetizadores

## Elegir un synth

```python
use_synth :prophet
play :C4
```
## Escalas
```python
scale(:c3, :minor_pentatonic).each do |nota|
  play nota
  sleep 0.25
end
```

## Melodía aleatoria
```python
live_loop :melodia do
  use_synth :blade
  play scale(:e3, :minor).choose
  sleep 0.25
end
```

