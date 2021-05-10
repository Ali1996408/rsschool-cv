# Markdown-Git
feat
First task, Ali Kermani, Markdown &amp; Git
First name: Ali, Last name: Kermani, 
Email: alikermani1959@gmail.com, Telegram id:  @AliK2134, Phone number: +989930243006
I studied electronics and having studying and working with different microcontrollers, but I got interested in android developing last year and started learning last year, but I focused on ARM lately. I would like to learn new things and apply them in my projects.
Skills: AVR microcontrollers, ARM microcontrollers, Android Studio, Matlab, Labview, Altium disgner, Proteus
Code example:
#include "lpc17xx_gpio.h"
const uint8_t segmentTable[]={0x3F,0x06,0x5B,0x4F,0x66,0x6D,0x7D,0x07,0x7F,0x6F};
void Delay ()
{
for(uint16_t count=0; count<UINT16_MAX; count++)
	for(uint8_t count2=0;count2<150; count2++)
	{
	}
	
}
void Delaylow ()
{
for(uint16_t count=0; count<UINT16_MAX; count++)
	for(uint8_t count2=0;count2<20; count2++)
	{
	}
	
}
int main ()
{
uint8_t pushCount =0;
FIO_ByteSetDir(1,2,0xFF,1);
GPIO_SetDir(0,(1<<1)|(1<<2)|(1<<3),1);
GPIO_SetDir(0,(1<<16),0);
GPIO_ClearValue(0,(1<<3));
GPIO_SetValue(0,(1<<2));
GPIO_SetValue(0,(1<<1));


while(1)
{	
uint32_t temp=GPIO_ReadValue(0);
if(((temp>>16)&0x01)==0)
{
	//key pressed
uint8_t countOfTrue=0;
for(uint8_t count=0;count<10;count++)
	{
		if(((GPIO_ReadValue(0)>>16)&0x01)==0)
		countOfTrue++;
		Delaylow();
		
	}
	if(countOfTrue==10)
	{
		pushCount++;
    if(pushCount==10)

	  pushCount=0;
	  FIO_ByteSetValue(1,2,segmentTable[pushCount]);
	  FIO_ByteClearValue(1,2,~segmentTable[pushCount]);
	  while(((GPIO_ReadValue(0)>>16)&0x01)==0);
	}
	

	 
}

	
}	
}
I've been working in a medical university on several bioengineering projects, I've finished an ARM course, I've learned other softwares like Matlab, Labview, Altium by myself.
I graduated from University of Isfahan in 2020 and now I'm persuing my masters.
I never took English tests like TOFEL, but I can say that my English Level is relatively good and I can speak it fluently. With the help of English I read different articles, datasheets, and even languages. I learned Russian and some German too. I've been teaching my native language on italki. That's why I think my English is advanced. 
