
## Ejercicio 1: escriba una aplicación para resolver el siguiente enunciado. El gobierno ha implementado como parte de su programa social, un subsidio familiar bajo la siguiente reglamentación:

## Las familias que tienen hasta 2 hijos, reciben Q. 70.00, las que tienen hasta 3 y 5 reciben Q. 90.00 y las que tienen 6 o más reciben Q. 120 mensual. Por cada hijo en edad escolar reciben Q. 10.00 adicionales. Se considera la edad escolar entre 6 y 18 años. Si la madre de familia fuera viuda, la familia recibe Q. 20.00 adicionales



# c++
``````c++
#include<iostream>
using namespace std;

int main(){
int a, b;
char estado_civil;
	
int calcular_subsidio;

	* cout<<"estado Civil de la madre: C=CASADA, S=SOLTERA, V=VIUDA    ";
	cin >>estado_civil;
	cout<<" Cuantos hijos tiene   ";
	cin>>a;
	cout<<" Cuantos hijos tiene estudiando en edades de 6 a 18 años ";
	* cin>>b; 	
		if (a<=2){
		calcular_subsidio=70;
		 		
	}	else if(a>=3 && a<=5){
	
		calcular_subsidio=90;
	
	}	else if(a>=6){
		calcular_subsidio=120; 
		
	}
		if (estado_civil =='V' || estado_civil == 'v'){
			calcular_subsidio += 20;
	}
		calcular_subsidio += b * 10;
	  	cout<<"la cantidad a recibir es de   " << calcular_subsidio <<endl;
	  	
		
	return 0;
}
``````

# PHYTON
``````c++

estado_civil = input("Estado Civil de la madre: C=CASADA, S=SOLTERA, V=VIUDA: ")
a = int(input("Cuantos hijos tiene: "))
b = int(input("Cuantos hijos tiene estudiando en edades de 6 a 18 años: "))

calcular_subsidio = 0

if a <= 2:
    calcular_subsidio = 70
elif 3 <= a <= 5:
    calcular_subsidio = 90
elif a >= 6:
    calcular_subsidio = 120

if estado_civil.lower() == 'v':
    calcular_subsidio += 20

calcular_subsidio += b * 10

print("La cantidad a recibir es de:", calcular_subsidio)

#   g o b i e r n o  
 