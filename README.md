# hospital_food
m4l impression of nlc's [let's splosh](http://nonlinearcircuits.blogspot.com/2018/04/lets-splosh.html), designed for @andrew's growing m4l collection.

![screenshot](https://llllllll.co/uploads/default/original/3X/d/4/d48f13b10129f47fd9e749449b4dcafd06ef5417.png)

I've been in the hospital for the last few days with a perforated appendix and while the nursing staff has been nothing but sweet, engaged and fun, the first 40 hours were super boring. when racquel was able to visit again, she brought my computer and I dove deep into the m4l tools that andrew has been releasing. they're absolutely incredible.

the only thing I wished for was a control / modulation layer. I love nlc's 'let's splosh', so I took the basic maths of the schematic and flipped it into a lil' m4l device that has plenty of mappings to control yr faves from andrew's suite!

[sounds demo](https://soundcloud.com/sound-and-process/hospital_food-demo/s-W8NQ0)

the four foods have been renamed to the items I was allowed on my liquid diet:

`GELATIN`
`SHERBET`
`JUICE`
`BROTH`

the device is basically made of four `cycle~` objects following this comparator:
![formulas](https://llllllll.co/uploads/default/optimized/3X/1/d/1d9a0eecb718599c52e69059ad52f1b45fdb8e52_2_690x116.jpeg)

### Requirements

Ableton Live
Max for Live
[any of the m4l devices andrew's released](https://llllllll.co/search?q=category%3A18%20%40andrew) (recommended)
restricted
### Documentation

- load up `hospital_food.amxd` on any track in Live.
- the two number boxes underneath each food will determine the frequency of each `cycle~` device under the hood.
- the first box (float) will help keep things lfo-y. the second box (integer) is there as a multiplier, to help things get weird if you need it.
- once you have some float values selected for each food, you'll see the matrix of black boxes in the main part of the device rise, fall, and jump. it's working!
- to use these modulations, click `Map` and select the parameter on any device you'd like. you can even map `hospital_food` back onto itself! I like modulating two of the floats while keeping the other two constant.
- use the attenuators above each `Map` button to keep things "musically useful" -- I found that small modulation ranges can sometimes lead to more dramatic effects than big jumps, especially with filter cutoffs.
