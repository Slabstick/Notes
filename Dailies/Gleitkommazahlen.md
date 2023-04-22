
## 1) Welche der folgenden Datentypen stellen eine Gleitkommazahl in Java dar?

Hier sind float und double richtig. Float benutzt 32 Bit und double benutzt 64 Bit, wodurch Kommazahlen genauer gespeichert werden können.

## 2) Wo steht der Exponent in der Binärrepräsentation einer 32-Bit Gleitkommazahl?

Der Exponent ist Bit 2 bis Bit 9, also insgesamt 8 Bits. In der folgenden Zahl mit "x" dargestellt:

0 xxxx xxxx 000 0000 0000 0000 0000 0000  

## 3) Wo steht die Mantisse in der Binärrepräsentation einer 32-Bit Gleitkommazahl?

Die Mantisse ist der Teil ab Bit 10 bis zum Ende, also insgesamt 23 Bits. In der folgenden Zahl mit "x" dargestellt:

0 0000 0000 xxx xxxx xxxx xxxx xxxx xxxx

## 4) Wo steht die Basis in der Binärrepräsentation einer 32-Bit Gleitkommazahl?

Das war eine Fangfrage. ![🙂](https://statics.teams.cdn.office.net/evergreen-assets/personal-expressions/v2/assets/emoticons/smile/default/30_f.png?v=v81) Die Basis ist für das Binärsystem 2 und steht nicht in der Repräsentation. Wär ja auch Quatsch, die zu speichern, wenn die eh festgelegt ist.

## 5) Welche anderen Bestandteile stecken in der Binärrepräsentation einer 32-Bit Gleitkommazahl und wo stehen sie?

Das erste Bit stellt das Vorzeichen dar. 0 bedeutet eine positive Zahl und 1 bedeutet eine negative Zahl. In der folgenden Zahl mit "x" dargestellt:

x 0000 0000 000 0000 0000 0000 0000 0000

## 6) Was ist die Mantisse?

Die Mantisse ist die Zahl, die mit der Zweierpotenz verrechnet wird. Für die Gleitkommazahl 1,75 * 2^34 ist also "1,74" die Mantisse.

## 7) Welche Besonderheiten gibt es bei der Umrechnung des Exponenten ins Dezimalsystem?

Bei dem Exponenten ziehen wir 127 vom eigentlichen Ergebnis ab. 

Beispiel:

Bei der Zahl  
0 0010 1010 010 1000 0000 0000 0000 0000

ist der Exponent 0010 1010. Direkt ins Dezimalsystem übersetzt entspricht das der Zahl 42. 

Dementsprechend ist der Exponent 42 - 127 = -85

## 8) Welche Besonderheiten gibt es bei der Umrechnung der Mantisse ins Dezimalsystem?

Die Mantisse drückt für Gleitkommazahlen im Binärsystem ja eine Dezimalzahl ab 1 und unter 2 aus, also z.B. 1,234; 1; 1,9999; 1,5; etc.

Durch diese Begrenzung steht vor dem Komma immer eine 1. Die wird gar nicht erst gespeichert, also speichert die Mantisse in der Binärrepräsentation nur die Nachkommastellen der "eigentlichen Mantisse".

Die (ersten paar) Stellen der Mantisse haben folgende Werte: 

Stelle | Zweierpotenz | Zahlenwert

1 | 2^-1 | 0,5
-|-|-
2 | 2^-2 | 0,25
3 | 2^-3 | 0,125
4 | 2^-4 | 0,0625
5 | 2^-5 | 0,03125
... | | 


Wie man in der Spalte "Zahlenwert" sieht, halbiert sich der Wert mit jeder Stelle.

**Beispiel**:

Bei der Zahl  
0 0010 1010 010 1000 0000 0000 0000 0000

ist 010 1000 0000 0000 0000 0000 die Mantisse.

Die zweite und die vierte Stelle der Mantisse sind 1. Für diese Stellen rechnen wir die entsprechenden Werte aus der Tabelle zusammen:

2^-2 + 2^-4

= 0,25 + 0,0625

= 0,3125

Wie bereits erwähnt, spart man sich die "1" vor dem Komma, die Mantisse entspricht also der Zahl **1,**3125.