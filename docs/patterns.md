
# 🔁 Patrones


## Ritmo euclidiano

```python
live_loop :euclidiano do
  sample :bd_haus if spread(3, 8).tick
  sleep 0.25
end
```

## Patrón de bajo
```python
live_loop :bajo do
  use_synth :tb303
  play (ring :e2, :e2, :g2, :b1).tick
  sleep 0.5
end
```