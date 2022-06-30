# futuretrash
assets for futuretrash

# Hardware Setup

Navation Launchpad as MIDI controller for vocal effects, lights and 


```mermaid
flowchart LR

dmxctrl[DMX USB] --- lightctrl
launchpad --- ableton
ai[audio interface] --- ableton
dtx[drum brain] -- midi --- ai

lb1 --- dmxctrl
lb1(lightbar left) --- lb2(lightbar right)

subgraph PC (macbook)
  ableton(ableton) -- IAC midi --> lightctrl(qlc+)
end
```


# Software Setup

Lighting control over DMX requires lighting controller software. A free version that appears to work well is qlc+.
[Install qlc+](https://www.qlcplus.org/). Version 4.12.5

For communicating between Ableton and qlc+ - a virtual midi bus is needed
[Install IAC Driver](https://help.ableton.com/hc/en-us/articles/209774225-Setting-up-a-virtual-MIDI-bus)

