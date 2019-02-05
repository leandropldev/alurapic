#Curso Angular 6 (Parte 1)

Carregar bootstrap no projeto:
	1 - baixar o bootstrap na pasta do projeto: npm install bootstrap@4.1.1
	2 - vincular o bootstrap com o angular, através do arquivo angular.json	
		no item "styles", adicionar o registro:
			"styles": [
				"src/styles.css",
				"./node_modules/bootstrap/dist/css/bootstrap.min.css"
			],
			"scripts": []
			