# Ladestrategie und Grundlagen
Die LiPo-Akkus bestehen aus mehreren Zellen (z.B. 4S: 4 Zellen in Reihenschaltung). Die Packs haben kein Batterymanagementsystem (BMS), daher muss das Ladegerät durch Messung der einzelnen Zellen und Balancieren dafür sorgen, dass die Zellen am Ende des Ladevorgangs die gleiche Spannung haben, welche durch unterschiedliche Innenwiderstände der Zellen hervorgerufen werden. Zellen mit niedrigerem Innenwiderstand nehmen so mehr Energie auf und haben dadurch eine höhere Spannung.  
Die Zellen haben einen sicheren Arbeitsbereich von 3.0V...4.2V. Diese Spannungen sollten die Zellen nicht unter- bzw. überschreiten. Die **Lagerspannung** beträgt **3.8V**. 
Die Akkupack-Spannungen sind entsprechend ihrer Anzahl von Reihengeschalteten Zellen zu errechnen (z.B. 6S: 6 * 3.0V...4.0V = 18.0V...25.2V).  
Bereich/Konfiguration| 1S | 4S | 6S
---|---|---|---
Minimum|3.0V|12.0V|18.0V
Maximum|4.2V|16.8V|25.2V
Lagerspannung|3.8V|15.2V|22.8V
</br>

Ladegeschwidigkeiten werden häufig in Relation zur Kapazität (C) angegeben. Die Akkus können problemlos mit 1C, also mit einer Stromstärke nahe ihrer Kapazität innerhalb von ca. 1 Stunde geladen werden (vgl. [Venom Specs](https://www.venompower.com/venom-22000mah-6s-22-2v-drone-professional-battery-15c-lipo-with-xt150-as150-35000)). Falls mehr Zeit vorhanden ist, sollte aber der maximale Strom reduziert werden (z.B. gegen 0.5C).  

Kapazität| 14000mAh | 22000mAhS
---|---|---
0.5C|3.5A|11A
1.0C|14A|22A
</br>

Ein hoher Ladestand (SoC - State of Charge) sollte nicht über einen langen Zeitraum bestehen - hier werden die Zellen geschädigt (SoH - State of Health reduziert sich).

## Konfiguration als 2P
Sowohl für beide ESCs (electronic speed controller) als auch für die Stromversorgung der Sensoren und des PCs werden die Akkus jeweils parallel (2P) mittels "Y-Adapter" (XT90) verbunden. Hier ist darauf zu achten, dass die jeweiligen beiden Akkus die gleiche Spannung haben. Spannungsunterschiede würde bei der direkt Verbindung der Akkus zu enorm hohen Strömen führen und könnten die Akkus schädigen. Sofern die Akkus mittels ISDT Safe Parallel Board zusammen geladen worden sind, ist davon auszugehen, dass die Spannung angeglichen sind. Beim getrennten Ladevorgang sollte voher noch mittels Multimeter oder Battery Checker die Gesamtspannung geprüft werden.

## Sicherheit
Kurzschlüsse sind unbedingt zu vermeiden. Die Zellen können kurzzeitig mehrere hundert Ampere liefern, was ggf. zu starker Hitzeentwicklung führen kann und die Zellen auf jeden Fall schädigt. Ein Verpolen der XT90-Stecker ist unter normalen Umständen jedoch nicht möglich.
Beim Anschließen der Balancerkabel ist auf korreken Anschluss zu achten! Die Balancer-Kabel sind nicht verpolungssicher. Eine Verpolung hier kann zu Schäden an der angeschlossenen Elektronik und dem Akku führen. 
Mechanische Beschädigungen der Zellen und Anschlusskabel können je nach Grad die Zelle unzuverlässig machen und eine sichere Nutzung ausschließen. Daher ist bei Gebrauch der äußere Zustand der Zellen und Anschlusskabel visuell zu prüfen.