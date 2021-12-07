# Hej kodare!

En låt! Med ackord och bas!

Men basen låter nog lite tråkig.

```
use_bpm 120


# Ackord betyder att man spelar vissa toner tillsammans


live_loop :ackord do
  use_synth :square
  
  ett = chord(:C4, :major)
  tva = chord(:F4, :major)
  tre = chord(:G4, :major)
  
  
  play ett, release: 2
  sleep 4
  
  play tva, release: 2
  sleep 2
  
  play tre
  sleep 1
  
  play tva, release: 2
  sleep 1
  
end


live_loop :bas do
  use_synth :fm
  bastoner = [:C3,:G3,:F3]
  play :C3, release: 0.25
  sleep 1
end

sleep 24

live_loop :trummor do
  sample :loop_breakbeat, beat_stretch: 4
  sleep 4
end
```
   
