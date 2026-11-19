# Intentional camera movement in Arcana

Intentional camera movement (ICM) moves the camera while the shutter is open, so the picture becomes strokes of
light and colour around what stays sharp. Arcana makes it two ways. From a **picture**, it simulates the camera
gesture over the still. From a **clip**, it sums the clip's real frames in linear light, as a camera with its
shutter open that long would have recorded them, and can add a gesture of its own over them.

Both live in **Alchemy · ICM**. Alchemy works on one medium at a time, chosen by the **Pictures | Video** switch
at the start of its bar: Pictures holds Blend and ICM, and Video holds ICM, Colour, Film and Rhythm. A picture is
recoloured in Blend, with the colour family, where the mask can keep the new colours to one part. ICM on
Pictures shows only pictures, and ICM on Video only clips. Sending a clip to ICM opens the Video side, and a
picture the Pictures side.

## Getting a picture or a clip in

- **ICM selected** in Search or the Moodboard sends the selected pictures or clips.
- **ICM** in the viewer sends what it shows.
- **ICM** on a finished video in Generate · Video sends that video.
- **Collection** lists the active collection's pictures and clips, and **Made here** lists finished video batches.
- **Sent here** keeps what was sent until "Clear this list", across a reload.

Clips carry a small "clip" badge in the list. When a list holds both, "All", "Pictures" and "Clips" show one
kind at a time.

The dataset chosen in the header sets where Search and the map look. The collection sets what the making tabs
work from, and it can mix pictures and clips from any dataset, so a clip found in a video dataset and a photograph
from a photo dataset can sit in one collection and both reach ICM. The header counts the collection's pictures
and clips.

## A clip

1. **Pick a technique.** The chips are grouped by family. Each shows what it does, and the panel says whether the
   result is an exposure "as an open shutter would" record it or "a composite of moments".
2. **Place the window.** The strip beside the clip shows how much it moves every quarter second. The window opens
   on the busiest stretch, at the length the technique reads best over. Drag along the strip to move it, type a start
   and a length, or use "Busiest stretch" and "Start at the playhead". The player loops the window.
3. **Adjust.** Every setting stays open, grouped as Camera movement, Shutter, Light, What stays sharp and How
   moments combine. A dot marks a group with settings changed from the technique, and "Back to the preset"
   undoes them. Settings a technique ignores are hidden.
4. **Watch the preview.** Beside the clip, the exposure redraws as you edit. A draft (360 px, every second
   frame) answers each change in a fraction of a second, and a finer preview (the same frames with the fill
   between them) follows about a second after the edits stop. The first preview of a window reads its frames, which
   takes about a second. A thin bar along the top of the preview runs while it updates. "live preview" turns it
   off. The preview stays in view while the settings scroll beneath it.
5. **Expose.** Quick renders at 960 px, Full size at 1920 px, from every frame. A still takes from a few seconds
   to half a minute, and a moving clip about a minute for four seconds. The job's bar shows each step.

## A picture

1. **Pick a technique.** The chips head the settings column on the right: the camera movement, colour movement,
   double exposure, driven by a picture and moved by a clip recipes, and your own under "Yours". The settings below them adjust what the chip set, and
   "keep these settings as a technique" adds the result as a new chip. The pictures on the left come from the
   collection or set chosen in "From" (or the header), and either works.
2. **Watch the stage.** It draws each change, with the before and after split by a line you drag. While a slider
   moves, the stage answers at once with a draft at 512 px, marked "draft" on the after tag, and redraws at the
   chosen preview size once the hand rests. A bar along the top runs while it draws. Slow methods draw on Draw.
3. **Adjust.** The settings column holds the camera methods, the mask (what stays sharp or where the movement
   shows) and the finish.
4. **Double exposures** and the techniques **driven by a picture** take a second picture. Choosing one without
   it asks for it, and the next picture clicked in the list on the left becomes the second, marked "2nd". "Change
   the second picture", under those chips, picks another. The techniques **moved by a clip** take a clip instead.
   While one waits for its clip, the list on the left shows the collection's clips too, and the clip clicked moves
   the picture. Each finds its moment of the clip by itself, and its "moment" setting picks one by hand.
5. **Keep** saves the picture to the archive and the collection. **Make it a moving clip** turns the picture into
   a clip along a camera movement recipe, its streaks travelling as a window slides along the gesture.

The picture and its materials are shared with Alchemy · Blend, and each sub-tab keeps its own method, so moving
between them loses nothing.

## Where the movement shows

A mask decides where the movement shows, separately from the movement itself. Pictures and clips use the same
masks: up to three layers met by "and", "or" or "but not", an invert, a soft edge, and one of two uses.

- **The movement shows only here.** The masked places move, the rest stays as it was.
- **This holds still, the rest moves.** The masked places stay sharp inside the movement.

A layer is a preset (light, colour ranges, depth, things and stuff, geometry, patterns), words such as "red
coat", or one of the colour layers.

- **A band of hue** takes one family of colours, of any lightness, and leaves greys out. Drag along the colour
  strip to move the band and set its width. The presets reds, oranges, yellows, greens, cyans, blues, purples and
  magentas are bands of hue.
- **A colour** takes the places near one colour. "How near" goes from that colour only to a wide family. The
  eyedropper takes the colour from the picture, or from the clip at its current frame.
- **Vivid** and **pale** take the strongly coloured places and the lightest ones.

On a clip, colour, light and geometry layers can follow the clip: the mask is cut again on every frame, so a red
coat crossing the frame carries the movement with it while everything else stays sharp. Words and things are
found once, on the middle frame. "Show the mask" draws the mask over the clip before an exposure is made, the
movement in gold.

On a picture the mask lives in the settings column's Mask section, and "mask" in the method's settings chooses
between the two uses.

## Results

"Your ICM results" lists everything made in ICM, newest first: kept pictures, still exposures of clips and moving
clips. It shows the results of the picture or clip on the stage, and the switch beside the title shows them all.
"Use settings" puts a result's source, window and settings back in the panel. "Send to Film" adds it to the film.

## Clip techniques

**Exposure**

| Technique | Clip | What it does |
|---|---|---|
| long exposure | 1 s | The clip's own movement exposed for a second, as an open shutter takes it. |
| steadied exposure | 1.5 s | The clip's shake removed first, so only what moved in the scene blurs. |
| light trails | 1.5 s | The brightest copy wins, so lights draw lines over a calm frame. |
| dark trails | 1 s | The darkest copy wins, so shadows and dark forms draw the lines. |
| flash first | 1 s | A sharp flash at the start, the movement trailing after it. |
| flash last | 1 s | The movement trails into a sharp flash at the end, as rear-curtain sync gives. |
| stop, move, stop | 1 s | Held, swept down, held again, two sharp impressions joined by a stroke. |
| vertical sweep | 1 s | The shake removed and a vertical sweep added, its lights lifted, with glow. |
| zoom burst | 0.8 s | The shake removed and a zoom added through the exposure, its lights drawn out. |
| turn | 0.8 s | The shake removed and the frame turned 20 degrees about the centre. |

**Stacks**

| Technique | Clip | What it does |
|---|---|---|
| lighten stack | 3 s | Each place keeps its brightest moment over three seconds, as star trails are made. |
| median stack | 2 s | Each place keeps its middle value over two seconds, so what passes through vanishes. |
| darken stack | 2 s | Each place keeps its darkest moment over two seconds. |

**Time**

| Technique | Clip | What it does |
|---|---|---|
| slit-scan | 2 s | Each column comes from a later moment, so the horizontal axis becomes time. |
| echoes | 1.6 s | Six moments laid over each other, each older one fainter. |
| time-warp by light | 1.4 s | Bright places come from later moments and dark places from earlier ones. |
| chronophotography | 8 s | Seven moments, each moving part laid over the still background, the earliest faintest. Up to 40 s of clip. |
| orbit composite | 5 s | Ten views of one subject aligned on it and blended, so it holds while the surroundings swing around it. |

**Held parts**

| Technique | Clip | What it does |
|---|---|---|
| follow | 0.8 s | The clip steadied on the tracked subject, so it stays sharp while the world streaks. It needs a subject. |
| subject held | 0.8 s | The subject kept sharp while the rest sweeps sideways. It needs a subject. |
| stillness held | 1 s | What barely moved stays crisp while what moved streaks. |
| near held | 0.8 s | Near things sharp while the distance sweeps. |
| far held | 0.8 s | The distance sharp while the foreground sweeps. |
| edges held | 0.8 s | Strong edges stay while the open areas flow down. |
| horizon | 1 s | The bottom holds sharp while the top sweeps across. |

**Colour**

| Technique | Clip | What it does |
|---|---|---|
| only the reds move | 1 s | The shake removed and a sideways sweep added, shown only where the reds are, frame by frame. |
| warm lights streak | 1.5 s | The clip's own movement exposed only in its warm lights, which draw trails over a sharp frame. |
| blues hold still | 0.8 s | The shake removed and a downward sweep added, the blues held sharp inside it. |
| vivid sweeps | 1 s | A diagonal sweep shown only in the strongly coloured places, the greys and pale places sharp. |

**Moving clip**

| Technique | Clip | What it does |
|---|---|---|
| moving ICM | 4 s | A clip in which every frame carries its own fading trails, the current frame laid sharp over them. |

## Picture recipes

**Camera movement**

| Recipe | What it does |
|---|---|
| vertical sweep, violet glow | A vertical sweep with the picture's detail kept and a soft glow, in cool violet, as an ICM marina. |
| stop, move, stop | Held still, moved down, held again, two sharp impressions joined by the movement. |
| zoom burst | The camera zoomed in during the exposure, the lights drawn out as rays. |
| swirl | The camera turned about the centre, and everything circles it. |
| crossing strokes | Three sweeps fanned across directions over a held sharp impression, warm and soft. |
| edges hold | A sideways sweep in which strong edges stay and the spaces between them flow. |
| light streaks over the dark | The picture's lights drawn down across a still dark subject, as a flash closing a long exposure. |
| carved strokes | Short strokes that follow the picture's own contours, its edges held. |
| painted water | Strokes that follow the water's own lines, its light leading, with a soft glow. |
| held in fog | The subject held sharp while the world around softens, drags down and hazes. |
| the world turns about them | The subject held sharp while everything else turns about them. Set the pivot on them. |
| held among strokes | People held sharp inside three crossing sweeps, warm and soft. |
| strokes all over | Three crossing sweeps over the whole frame, the picture dissolved into warm brushwork. |
| tremor sweep | A vertical sweep with a hand's uneven shake, its lights lifted above white. |
| sweet spot turn | A sharp soft ellipse at the centre while the field around it turns and blurs, with glow. |
| performed path | A curving gesture with its own pace. The camera rests, moves slowly, hurries, pauses and finishes slowly, each pause a sharp impression inside the streaks. |

**Colour movement**

| Recipe | What it does |
|---|---|
| only the reds move | A sideways sweep shown only where the reds are, everything else sharp. |
| warm lights streak | The warm lights drawn down in streaks over a sharp picture. |
| blues hold still | The picture turned about the centre while its blues stay sharp. |
| vivid sweeps | A diagonal sweep in the strongly coloured places, greys and pale places held. |

**Double exposure** (each takes a second picture [1])

| Recipe | What it does |
|---|---|
| streaming light | The second picture swept sideways and screened over the whole first. |
| falling through | The second picture falls down through the first, the darker of the two kept at each place. |
| a field of colour | The second picture softened into a field of colour and light behind the first. |
| into the light | The second picture swept into the first's lighter half only, as a sky turning to water. |
| in shadow | The second picture multiplied in and drawn down, both darkening into one relief. |
| falling light | The second picture's light falling down over the first, softened and screened in. |
| turning double | The second picture turned about the centre and screened over the first. |
| two veils | The first sweeps across and the second sweeps down, averaged into one woven veil. |
| horizon of two | The second picture, swept sideways, fills the top of the frame and fades into the first below. |
| layered exposure | The first picture sharp, the same picture swept down around its subject and near ground, and the second picture turning, screened over the top. |

**Driven by a picture** (each takes a second picture [1], which decides where and which way the first moves)

| Recipe | What it does |
|---|---|
| light map | The second picture's bright places sweep the whole way and its dark places hold. |
| colour compass | The second picture's hue sets the direction and its colourfulness the amount. |
| borrowed contours | Each place moves along the second picture's forms, its dunes, waves, bark or veins. |
| cross-currents | The second picture's reds move down, and everything else moves across them, weaker. |
| colour streaks | The streaks take the second picture's colours, and still places keep their own. |
| exchange | Each picture streaks along the other's forms, and the two are screened together. |

**Moved by a clip** (each takes a clip [1])

| Recipe | What it does |
|---|---|
| borrowed flow | Each place streaks the way the clip moved there at its busiest moment. |
| carried by the clip | The picture rides the clip's surface for 1.6 s, so the strokes bend as the water turned. |
| colour-matched flow | At the moment whose colours match the picture's best, each colour moves as that colour moved in the clip. |

**Looks** (finishes that stack on any technique)

| Recipe | What it does |
|---|---|
| Orton glow | A sharp copy brightened by about a stop, multiplied by a soft copy and laid over the picture, the darks kept. |
| bloom and grain | The lights bloom with a long falloff, then film grain in the midtones. |

## Choosing a clip

The techniques read best on clips with clear movement. Water, lights at night, foliage in wind, birds, people
walking and a panning camera all work well. A still clip gives a sharp picture under every exposure technique,
and the time techniques need something that changes. Follow and subject held need a subject the panel can find
(a person, an animal, a vehicle), and they say so when none is there.

## From the command line or an agent

The panel's techniques are named presets of the camera ops:

```
camera presets
camera busiest clips@video:4 --seconds 1.5
camera expose clips@video:4 --start 2 --preset "light trails"
camera expose clips@video:4 --start 2 --end 3 --preset "light trails" --highlights 0.4
camera expose-video clips@video:4 --start 0 --preset "moving ICM"
camera mask clips@video:4 --start 2 --end 3 --mask reds --each-frame
camera preview clips@video:4 --start 2 --end 3 --preset "light trails" --quality draft
camera expose clips@video:4 --start 2 --end 3 --sweep 0.15 --mask hue:20,50 --mask highlights --each-frame
camera animate rated4:85 --recipe "painted water" --seconds 4
camera recent
```

A preset sets only the settings given nowhere else, and its length of clip when `--end` is left out. Pictures
use Alchemy's ops with a camera method or recipe (`alchemy preview`, `alchemy make`, `alchemy recipe list`).

## Limitations

Stacking frames of a clip differs from one continuous exposure. Each frame was itself a short exposure with gaps
between frames, and Arcana fills those gaps along the optical flow, so very fast movement can show steps.
Follow and subject held depend on finding the subject in a frame. Depth for near held and far held is estimated
from one frame and is relative.
