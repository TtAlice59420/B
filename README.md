/*
 * Generated using BlocklyDuino:
 *
 * https://github.com/MediaTek-Labs/BlocklyDuino-for-LinkIt
 *
 * Date: Wed, 19 Jun 2019 12:17:56 GMT
 */

#include <LRemote.h>

LRemoteLabel label1;
LRemoteButton button1;
LRemoteSwitch switch1;
LRemoteSlider slider1;
LRemoteCircleButton circle1;

void setup()
{
  LRemote.setName("TtAlice59420");
  LRemote.setOrientation(RC_PORTRAIT);
  LRemote.setGrid(5, 6);
    label1.setPos(0, 0);
    label1.setText("TEST");
    label1.setSize(5, 1);
    label1.setColor(RC_BLUE);
    LRemote.addControl(label1);

    button1.setPos(0, 1);
    button1.setText("PRESS  ME");
    button1.setSize(3, 2);
    button1.setColor(RC_YELLOW);
    LRemote.addControl(button1);

    switch1.setPos(3, 1);
    switch1.setSize(2, 2);
    switch1.setText("OPEN");
    switch1.setColor(RC_ORANGE);
    LRemote.addControl(switch1);

    slider1.setPos(0, 3);
    slider1.setSize(4, 1);
    slider1.setText("Value  Slider");
    slider1.setValueRange(0, 100, 1);
    slider1.setColor(RC_GREEN);
    LRemote.addControl(slider1);

    circle1.setPos(2, 4);
    circle1.setSize(2, 2);
    circle1.setText("BIG");
    circle1.setColor(RC_PINK);
    LRemote.addControl(circle1);
  LRemote.begin();
}
