.. ref_videofx:

***********************
moviepy.video.fx (vfx)
***********************
The module ``moviepy.video.fx`` regroups functions meant to be used with ``videoclip.fx()``.

Because this module is starting to be large and will be larger in the future, it allows two kinds of import.
You can either import a single function like this: ::
    
    from moviepy.video.fx.scroll import crop
    newclip = myclip.fx( vfx.crop, x1=15)

Or import everything: ::
    
    import moviepy.video.fx.all as vfx
    newclip = (myclip.fx( vfx.crop, x1=15)
                     .fx( vfx.resize, width=200)
                     .fx( vfx.freeze_at_end, 1))


When you type ::
    
    from moviepy.editor import *

the module ``video.fx`` is loaded as ``vfx`` and you can use ``vfx.colorx``, ``vfx.resize``, etc.


.. currentmodule:: moviepy.video.fx.all

.. autosummary::
    :toctree: videofx
    :nosignatures:
    
    blackwhite
    blink
    colorx
    crop
    fadein
    fadeout
    freeze_at_end
    freeze_at_start
    gamma_corr
    headblur
    loop
    lum_contrast
    make_loopable
    margin
    mirror_x
    mirror_y
    painting
    resize
    rotation
    scroll
    speedx
    time_mirror
    time_symetrize


   
