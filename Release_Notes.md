


# **Release Notes for STM32H735G-DK BSP Drivers**
Copyright &copy; 2019 STMicroelectronics\
    
[![ST logo](_htmresc/st_logo_2020.png)](https://www.st.com)


# Purpose

The BSP (Board Specific Package) drivers are parts of the STM32Cube package based on the HAL drivers and provide a set of high level APIs relative to the hardware components and features in the evaluation boards, discovery kits and nucleo boards coming with the STM32Cube package for a given STM32 series.


The BSP drivers allow a quick access to the boards’ services using high level APIs and without any specific configuration as the link with the HAL and the external components is done in intrinsic within the drivers. 


From project settings points of view, user has only to add the necessary driver’s files in the workspace and call the needed functions from examples. However some low level configuration functions are weak and can be overridden by the applications if user wants to change some BSP drivers default behavior.


# Update History

<label for="collapse-section7" aria-hidden="true">__V1.2.4 / 11-September-2026__</label>
<div>

## Main Changes

- Resolve Clang uninitialized variable warnings in stm32h735g_discovery_ospi.c.
- Fix touchscreen HardFault in TS_EXTI_Callback() function.

</div>

<label for="collapse-section6" aria-hidden="true">__V1.2.3 / 04-September-2024__</label>
<div>

## Main Changes

- Update STM32H735G-DK BSP drivers to support new Touch Screen component GT911.
- Apply general code Artistic Style fixes.

</div>

<label for="collapse-section5" aria-hidden="true">__V1.2.2 / 19-February-2024__</label>
<div>

## Main Changes

- Invert argument order between definitions and declarations of I2C4_WriteReg() and I2C4_ReadReg().
- Fix timeout value in BSP_SD_WriteBlocks() API.
- Increase timeout compliantly to the SD Cards specification.

</div>

<label for="collapse-section4" aria-hidden="true">__V1.2.1 / 11-February-2022__</label>
<div>

## Main Changes

-  All source files: update disclaimer to add reference to the new license agreement.
-  Modified the address calculation in the BSP_LCD_FillRGBRect() function when USE_DMA2D_TO_FILL_RGB_RECT is enabled to suppress the display of a distorted shape instead of a rectangle when trying to draw a rectangle with a bigger height.
-  Cache maintained operation is included in the BSP_LCD_FillRGBRect() function to solve the display issue when USE_DMA2D_TO_FILL_RGB_RECT is enabled.
-  Fix supported latency type and delete Deep power feature for external RAM.
-  Add check on the audio OUT device to select the appropriate Output Device in the BSP_AUDIO_OUT_Init() function.
-  Fix Hard Fault in the BSP_AUDIO_IN_Init() function by adding the WM8994_Probe() function at the appropriate place.
-  Fix OSPI memory erasing issue in the BSP_OSPI_NOR_Erase_Block() function.

</div>

<label for="collapse-section3" aria-hidden="true">__V1.2.0 / 29-January-2021__</label>
<div>

## Main Changes

-  Minor typo fixes in comments

## Dependencies

-  Components/common v7.0.0

</div>

<label for="collapse-section2" aria-hidden="true">__V1.1.0 / 29-September-2020__</label>
<div>

## Main Changes

-	Add License.md file

## Dependencies

-	Components/common v7.0.0

</div>

<label for="collapse-section1" aria-hidden="true">__V1.0.0 / 19-May-2020__</label>
<div>

## Main Changes

-   First release of STM32H735G-DK BSP drivers  in line with STM32Cube BSP drivers development guidelines (UM2298) 

</div>


For complete documentation on <mark>STM32 Microcontrollers</mark> ,
visit: [[www.st.com](http://www.st.com/STM32