//#include <stdio.h>
//#include <stdlib.h>
//int a[2][100], i = 0;
//
//
//
//void insertie(void)
//{
//	printf("Introdu nodul:\n");
//	scanf_s("%d", &a[0][i]);
//	printf("Introdu parintele nodului:\n");
//	scanf_s("%d", &a[1][i]);
//
//	i++;
//}
//
//void cautare(void)
//{
//	int g = 0, j, nod_c;
//	printf("Introdu nodul:\n");
//	scanf_s("%d", &nod_c);
//
//	for (j = 0;j < i;j++)
//	{
//		if (a[0][j] == nod_c)
//		{
//			++g;
//		}
//	}
//
//	if (g == 1)
//	{
//		printf("Nod gasit.\n");
//	}
//
//	else
//		printf("Nodul nu este gasit.\n");
//}
//
//
//void stergere(void)
//{
//	int nod_sters, nod_tata, j, k;
//
//	printf("Introdu nodul pe care doresti sa il stergi: ");
//	scanf_s("%d", &nod_sters);
//
//	for(j=0; j<i; j++)
//		if (a[0][j] == nod_sters)
//		{
//
//			for (k = 0; k < i; k++)
//			{
//				if (a[1][k] == nod_sters)
//				{
//					nod_tata= a[0][k];
//				}
//			}
//			a[0][j] = nod_tata;
//		}
//}
//
//
//void parinte()
//{
//	int j, nod_cautat, nod_parinte;
//
//	printf("Introdu nodul a carui parinte doresti sa il cunosti: ");
//	scanf_s("%d", &nod_cautat);
//
//	for (j = 0; j < i; j++)
//	{
//		if (a[0][j] == nod_cautat)
//		{
//			nod_parinte = a[1][j];
//		}
//	}
//
//	printf("\nParintele nodului cautat este: %d.", nod_parinte);
//}
//
//
//void fratii()    //functioneaza doar daca nodul vizat e cel mai din stanga dintre fratii sai.
//{
//	int j, k, poz_parinte=0, nod_cautat, nod_parinte=0;
//
//	printf("Introdu nodul a carui frati doresti sa ii cunosti: ");
//	scanf_s("%d", &nod_cautat);
//
//	for (j = 0; j < i; j++)
//	{
//		if (a[0][j] == nod_cautat)
//		{
//			nod_parinte = a[1][j];
//			poz_parinte = j;
//		}
//	}
//
//	printf("\nFratii nodului sunt: \n");
//
//	for (k = (poz_parinte+1); k < i; k++)
//	{
//		if (a[1][k] == nod_parinte)
//		{
//			printf("%d ", a[0][k]);
//		}
//		
//	}
//}
//
//
//int main()
//{
//	int op;
//
//	do
//	{
//		system("cls");
//
//		printf("\nAlege dintre: \n");
//		printf("1. Introducere nod.\n2. Cautare nod.\n3. Stergere nod.\n4. Parinte nodului.\n5. Fratii nodului.\n6. Afisare inordine.\n7. Afisare preordine.\n8. Afisare postordine.\n9. Iesire.\n");
//		scanf_s("%d", &op);
//
//		switch (op)
//		{
//		case 1:
//		{
//			insertie();
//			getch();
//			break;
//		}
//
//		case 2:
//		{
//			cautare();
//			getch();
//			break;
//		}
//
//		case 3:
//		{
//			stergere();
//			getch();
//			break;
//		}
//
//		case 4:
//		{
//			parinte();
//			getch();
//			break;
//		}
//
//		case 5:
//		{
//			fratii();
//			getch();
//			break;
//		}
//
//		case 6:
//		{
//			printf("Cazul 6.");
//			getch();
//			break;
//		}
//
//		case 7:
//		{
//			printf("Cazul 7.");
//			getch();
//			break;
//		}
//
//		case 8:
//		{
//			printf("Cazul 8.");
//			getch();
//			break;
//		}
//
//		case 9:
//		{
//			printf("Iesire!");
//			getch();
//			break;
//		}
//
//		default:
//		{
//			printf("Optiune inexistenta!");
//			getch();
//			break;
//		}
//		}
//
//	} while (op != 9);
//
//	return 0;
//}
