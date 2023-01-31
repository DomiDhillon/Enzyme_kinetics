# Enzyme_kinetics

Modelling evolution of concentrations of reactants and product and the rate of the reaction.

## **1. Simple catalytic reaction**

### equation system

$$\frac{d[S]}{dt}=-k_1[E][S]+k_{-1}[ES]$$

$$\frac{d[E]}{dt}=-k_1[E][S]+(k_{-1}+k_2)[ES]$$

$$\frac{d[ES]}{dt}=k_1[E][S]-(k_{-1}+k_2)[ES]$$

$$\frac{d[P]}{dt}=k_2[ES]\equiv v$$

$[S]$ : substrate concentration <br>
$[E]$ : enzyme concentration <br>
$[ES]$: enzyme-substrate complex <br>
$[P]$: product <br>
$k_1$ : rate constante of ES complex formation <br>
$k_{-1}$ : rate constante of ES complexe dissociation <br>
$k_2$ : rate constante of product formation

### determination of vmax with Michaelis-Menten equation

$$ v=\frac{d[P]}{dt}=\frac{vmax[S]}{Km+[S]}$$

## **2. Competitive inhibitors**


$$\frac{d[E_{tot}]}{dt} = \frac{d[E_0]}{dt}= [E] + [ES] + [EI] = [E].(1+\frac{[S]}{K_M}+\frac{[I]}{K_I})$$

$$\frac{d[ES]}{dt} = \frac{[S]}{K_M}.(\frac{E_0}{1+\frac{[S]}{K_M}+\frac{[I]}{K_I}})$$

$$\frac{d[P]}{dt}=\frac{k_2[S][E_0]}{K_M (1+\frac{[S]}{K_M}+\frac{[I]}{K_I})} =\frac{k_2[S][E_0]}{K_M.(1+\frac{[I]}{K_I}) + [S]} = \frac{vmax[S]}{K_M\alpha+[S]}$$

$$\alpha = 1+\frac{I}{K_I}$$

Higher the $\alpha$, smaller amount of P will be formed. To increase alpha, either the initial concentration of the inhibitor should be large or constante of inhibition small. 

With enough of substrate, the original vmax can be achieved, because there will be enough of S to compete for the enzyme binding site.

![competitive_inh](https://user-images.githubusercontent.com/65451658/215441132-1b1906b9-c432-4902-bc57-e0d73f86b518.png)
