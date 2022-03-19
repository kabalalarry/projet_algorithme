# projet_algorithme
Résolution projet alogo
fonction triTableau(tab1, tab2)

	Variables : i, j, k, z, compteur, sizetab3 en entier
	Tableau: tab3 en entier

	Debut

		sizetab3 = longue(tab1) + longue(tab2)
		j = 2
		z = 1
		redim tab3[sizetab3]

		# la fusion de deux tableaux

		Pour s = 1 a longue(tab1)

			tab3[s] = tab1[s]

			compteur = compteur + 1

			s suivant
		Pour c = compteur a sizetab3

			tab3[c] = tab2[z]
			z = z + 1

			c suivant

		# Tri 

		TantQue j <= sizetab3

			i = j - 1
			k = tab3[j]

			TantQue i > 0 et tab3[i] > k 
				tab3[i+1] = t[i]
				i = i - 1
				fin TantQue

			tab3[i + 1] = k

			j = j + 1

		fin TantQue

		Retourne tab3

	fin
