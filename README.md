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
			
Components
	Convenção Angular:
		nome do arquivo: photo.component.ts
		nome na classe: export class PhotoComponent
	Todo component precisa ficar referenciado no modulo:
		app.modeule.ts:
			declarations: [
				AppComponent,
				PhotoComponent
			],
	No component informar:
		selector: tag que será chamada no app.componet
		templateUrl: caminho do arquivo html que tera o conteúdo da tag 
			Ex: templateUrl: 'photo.component.html'

Integração com Web API:
	Classe: HttpClient que é injetada no construtor do component
	A classe importada precisa de um 'provide'. Para isso, importar o modulo HttpClientModule no PhotosModule
	

Gerenciamento de Módulos
	Criar um modulo que irá conter todos os modulos "similares" a fim de simplificar a chamada de modulos em root

