# Hej kodare!
Nu får vi jobba med *variabler*

```
use_bpm 135
use_synth :subpulse

# byt mellan 1-130
# och kör koden!
bastrumma = 40
virvel = 120




live_loop :MOVE_IT do
  3.times do
    sample :bd_fat, amp: 4, lpf: bastrumma
    sleep 1
    puts 'I LIKE TO'
    sample :sn_generic, lpf: virvel
    sample :bd_fat, amp: 4, lpf: bastrumma
    sleep 1
  end
  sample :bd_fat, amp: 4, lpf: bastrumma
  puts 'MOVE IT'
  sleep 0.5
  
  sample :bd_fat, amp: 4, lpf: bastrumma
  sleep 0.5
  puts 'MOVE IT'
  sample :sn_generic, lpf: virvel
  sleep 0.5
  sample :bd_fat, amp: 4, lpf: bastrumma
  sleep 0.5
end

sleep 24
puts ' * I * LIKE * TO * MOVE * IT * MOVE * IT * '

live_loop :I_LIKE_TO do
  with_fx :ping_pong, phase: 0.275 do
    3.times do
      play 67, release: 0.4
      sleep 1
    end
    play 67, release: 1.2
    sleep 0.5
    play 74, release: 1.2
    sleep 0.5
    play 70, release: 0.8
    sleep 1
    play 70, release: 0.8
    sleep 1
    2.times do
      play 69, release: 0.4
      sleep 0.5
      play 72, release: 0.4
      sleep 0.5
    end
  end
end



```
