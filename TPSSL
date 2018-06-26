#include <ctype.h>
#include <stdio.h>
#include <string.h>



int main (int argc, char *argv[]){
	in	= fopen(argv[1],"r");
	char caracter;
	char * buffer[256];
	int flag=0;

	if(argc == 1){
		printf("\n(ERROR) Debe ingresar 1 nombre de archivo!\n");
		return -1;
	}
	if (argc != 2){
		printf("\n(ERROR) Número incorrecto de argumentos!\n");
		return -2;
	}
	if(in == NULL){
		printf("\n(File error) No se pudo abrir el archivo de Entrada.\n");
		return -3;
	}
	
	
	
	while(caracter = fgetc(in)!= EOF){  //mientras lea carac por carac marca el flag en 1 si son letras o letras + numeros(esto falta mejorarlo un toq)
		if(isalpha(caracter)){ 			// mientras el flag sea1 concatena cuando hay un espacio o algun carac de puntuacion imprime el buffer y lo devuelve a null para
			buffer =+ caracter;			// poder seguir leyebndo mas palabras
			flag =1;
		}
		if(isdigit(caracter)&& flag ==1)
			buffer =+ caracter;
			flag =1;
		}
		if(isspace(caracter)&&flag==1))
			printf("%s /n",buffer); //aca comparar con lista de palabras reservadas
			buffer=NULL;
			flag =0;
		}

	if(caracter =='+')     printf("%c",caracter); //deberia poner el flag a 0 tambien 
    if(caracter =='-')     printf("%c",caracter);
    if(caracter =='(')     printf("%c",caracter);
    if(caracter ==')')     printf("%c",caracter);
    if(caracter ==',')     printf("%c",caracter);
    if(caracter ==';')     printf("%c",caracter);
    if(caracter ==':')     printf("%c",caracter);
    if(caracter =='=')     printf("%c",caracter);

	}
	fclose(in);
	
	return 0;
}



int columna(char c){   //esto lo vamos a usar en lo que seria el automata para determinar si es lenguaje
    if(isalpha(c))  return 0;
    if(isdigit(c))  return 1;
    if(c =='+')     return 2;
    if(c =='-')     return 3;
    if(c =='(')     return 4;
    if(c ==')')     return 5;
    if(c ==',')     return 6;
    if(c ==';')     return 7;
    if(c ==':')     return 8;
    if(c =='=')     return 9;
    if(c == EOF)    return 10;
    if(isspace(c))  return 11;
    return 12;
}

void AnalizarArchivo(FILE *f ){  
    
}

