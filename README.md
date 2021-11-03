# SonicPi2021
Hej kodklubbare! Här får du **kopiera** ett dataprogram:

``` 
sample :bass_thick_c

live_loop :robot do
  3.times do
    sample :loop_electric, beat_stretch: 2, rate: - 1
    sleep 2
  end
  2.times do
    # prova med robot1, robot2 ... robot7 :)
    sample :mehackit_robot1
    sleep 1
  end
  
  
end


live_loop :bastrumma do
  sample :bd_808, amp: 4
  sleep 0.5
end


live_loop :melodi do
  use_synth :prophet
  # vi börjar med play 48!
  play 48
  sleep 0.5
  3.times do
    play 36
    sleep 0.5
  end
end

 ```
