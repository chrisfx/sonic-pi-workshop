
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

```python
### ========== KICK ==========
live_loop :kick do
  sample :bd_haus #, amp: 0.2, cutoff: 70
  sleep 2
end


### ========== ARP ==========
live_loop :arp, sync: :kick do
  use_synth :sine
  use_synth_defaults release: 0.3, amp: 0.5
  notes = (scale :d3, :minor_pentatonic, num_octaves: 2).shuffle
  play notes.tick
  sleep 0.25
end
```