# Rytm och melodi!
Hej kodare! 

Idag övar vi på flera liveloops samtidigt.
Ofta spelar man många instrument tillsammans.

Men vaför kan du inte höra alla trummorna..?


```
#################################################
# Gör din melodi här nedanför!                  #
#################################################

live_loop :min_melodi do
  play 60
  sleep 1
end

# Gör en till om du vill

live_loop :en_till_som_jag_vill do
  sleep 1
end

# Gör ännu flera - men kom ihåg sleep :)




#################################################
# Trummorna hittar du här!                      #
# Men varför hörs bara virveltrumman..?         #
#################################################
live_loop :bastrumma do
  #sample :bd_klub
  sleep 2
end

live_loop :virveltrumma do
  sleep 1
  sample :sn_dolf
  sleep 1
end

live_loop :hihat do
  12.times do
    #  sample :drum_cymbal_closed, cutoff: rrand(80,100)
    sleep 0.25
    
  end
  3.times do
    # sample :drum_cymbal_soft, cutoff: rrand(70,110), amp: rrand(0.6,0.9)
    sleep 0.25
  end
  #sample :drum_cymbal_open, amp: rrand(0.6,1)
end
```

