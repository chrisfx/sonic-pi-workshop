
# 🌊 Efectos


## Reverb

```python
with_fx :reverb, mix: 0.5 do
  play :C4
end
```

## Filtros

```python
with_fx :lpf, cutoff: 80 do
  sample :loop_amen
end
```

## Cadena de efectos

```python
with_fx :reverb do
  with_fx :echo, phase: 0.25 do
    play :E4
  end
end
```