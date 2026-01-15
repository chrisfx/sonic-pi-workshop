

# 🥁 Ritmo y Beats

## Samples de batería

```python
sample :bd_haus
sleep 0.5
sample :sn_dolf
```

## Sample House
```python
live_loop :house do
  sample :bd_haus
  sleep 1
end
```

## Samples y ritmo
```python
live_loop :beat do
  sample :bd_haus
  sleep 0.5
  sample :sn_dolf
  sleep 0.5
end
```
