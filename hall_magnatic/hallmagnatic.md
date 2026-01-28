# HALL MAGNATIC

Interruttore che reagisce alla presenza di un campo magnetico, accendendosi e spegnendosi. 
<table>
	<tr>
		<td>
			
## CODICE UTILE

```
int led = 13; //led integrato su arduino
int sensor = 3;
int val;

void setup()
{
	pinMode(led, OUTPUT);
	pinMode(sensor, INPUT);
}

void loop()
{
	val = digitalRead(sensor); //Read the sensor
	if(val == LOW) //when magnetic field is detected, turn led on
	{
		digitalWrite(led, HIGH);
	}
	else
	{
		digitalWrite(led, LOW);
	}
}
```
</td>
<td width="100">
</td>
<td>

<b>Schema di collegamento</b>
		<table>
			<tr>
				<td>
					Modulo
				</td>
				<td>
					Arduino
				</td>
			</tr>
			<tr>
				<td>
					S
				</td>
				<td>
					3
				</td>
			</tr>
			<tr>
				<td>
					Mezzo
				</td>
				<td>
					5V
				</td>
			</tr>
			<tr>
				<td>
					-
				</td>
				<td>
					GND
				</td>
			</tr>
		</table>
	</td>
	<td>
</td>
</tr>
</table>