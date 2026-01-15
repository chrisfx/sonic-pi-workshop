
# 🔥 Live Coding


## Estructura básica

```python
live_loop :bass do
  use_synth :fm
  play :e2
  sleep 1
end
```

## Sync o "side chain"
```python
use_bpm 110

# ------------------------
# Kick
# ------------------------
live_loop :kick do
  sample :bd_haus, amp: 2
  sleep 1
end

# ------------------------
# Off-beat HiHat
# ------------------------
live_loop :hihat do
  sync :kick
  sleep 0.5
  sample :drum_cymbal_closed, amp: 0.7, cutoff: 110
  sleep 0.5
end
```

