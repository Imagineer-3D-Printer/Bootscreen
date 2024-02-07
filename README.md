# Bootscreen
I have added a custom animated boot screen by using Windows Paint to create frame_x.bmp files. To generate the bitmap, I used [this website](https://marlinfw.org/tools/u8glib/converter.html)

## In this section, I have added frame time periods.
### Find this line in your bootscreen.h file

```C++
#ifdef CUSTOM_BOOTSCREEN_ANIMATED_FRAME_TIME

  // Each frame has its own custom duration
  const boot_frame_t custom_bootscreen_animation[] PROGMEM = {
    { custom_start_bmp,   200 }, 
    { custom_start_bmp1,  200 },  
    { custom_start_bmp2,  200 },  
    { custom_start_bmp3,  200 },
    { custom_start_bmp4,  200 },
    { custom_start_bmp5,  200 },
    { custom_start_bmp6,  200 },
    { custom_start_bmp7,   200 }, 
    { custom_start_bmp8,  200 },  
    { custom_start_bmp9,  200 },  
    { custom_start_bmp10,  150 },
    { custom_start_bmp11,  125 },
    { custom_start_bmp12,  100 },
    { custom_start_bmp13,  100 },
    { custom_start_bmp14,   100 }, 
    { custom_start_bmp15, 80 }
  }; 

