# Aprendendo Swift

## 📓 Tipos primitivos 

- [var] palavra reservada para declarar variaveis. OBS-(Após uma variavel ser armazenada com tipo primitivo nao e mais possivel armazenar de outro tipo).
- [let] palavra reservada para constantes.

### Sintaxe padrao de variaveis 
- [var/let] [nomevariavel] = [qualquer coisa]
- [var/let] [nomevariavel]: [TipoVariavel] = [valor da variavel do mesmo tipo da variavel]

 ![imagem sobre tipos primitivos](https://i.imgur.com/0svYKVl.png)

 - [Numeros Inteiro] -> Int -> [1245]
 - [Numeros reais] -> Flaot/Double  -> [1.2, 1.4, 5.2]
 - [Seguencia de caracteris] -> String -> "Gustavo"
 - [Valores boleanos] -> Bool -> True/False

 ### Converter tipos

 -  Todo entrada de dados e do tipo String por isso a nescessidade de coverter para o tipo em que deseja fazer a manipulacao. 
 -  A sintaxe padrao e: Tipo(nome da Varialvel). 
 -  Para converter (String para Int) --> 
 -  Para converter (String para Double) --> 
 
 
  ---

  ## ***Poo em Swift***

  - Programacao orientada a obejto(POO) e um paradigma de programcao que mudou a forma de criacao de software deixando mais robustos e eficientes, gerando menos esforco para manutencao e reutilizacao de codigo.
  - Neste conceito iremos aprender o que e uma clase, obejeto, herenca, polimorfismo e encapsulamento.

  ### Clase e obejtos

  1. Clases sao abastracoes do mundo real, que possuem caracteristicas e acoes. Em Poo Caracteristicas sao o mesmo que -> atributos(mesma coisa que variasveis) ja as acoes -> metetodos(mesma coisa que funcoes). Clases sao um tipo de dados complexo e e um reference type.

  - Objetos sao criacoes geradas a partir de uma classe, as clases sao moldeis e os obejostos sao criacoes a partir das clases que possuem sua proprias caracteristicas. 

  ![Imagem clases!](https://i.imgur.com/bULpnMw.png)
  
  - Vejamos que na linha 3 existe a palavra reservada [class] que endica que o codigo do bloco abaixo(Bloco = {}) e uma classe. Apos a declaracao da classe adicionamos seu nome que no caso do exemplo e [Animal], apos disso abrimos do bloco de codigo da clase e fechamos. Obs: Uma boa pratica e colocar a primeria letra do nome de uma classe maiscula

  - Apos a criacao da classe adicionamos os atributos[Linha: 5 a 7], como falei anteriormente atributos e o mesmo que variaveis e constantes, portanto a sintaxe e a mesma, entretanto nao adicionamos valores a elas no momento de sua criacao.
  
  - Entre a limha 10 a 14 temos um metodo construtor, falarei depois.

  - Entre a linha 17 a 23 temos os metodos que sao  acoes em nossas classes. Entre a linha 21 a 23 temos o metodo "estadoAnimal" que printa na tela se o animal esta acordado ou dormindo, entretanto nao e uma boa pratica colocar uma saida de dados fixa como esta nesta funcao, a melhor maneira e como esta na linha 17 a 19 que estaos passando um valor como parametro da funcao. Obs: a declaracao de um metodo e a mesmo de uma funcao.

  - Instanciar e o ato de criar um objeto a partir de uma classe[Segue abaixo a maneira]

  ![imagem de como inctanciar uma classe!](https://i.imgur.com/fYJlrBN.png)

  - Na linha 28 estamos criando um objeto chamado "cachorro" que instanceia da classe Animal. Entao o objeto cachorro contem todas as caracteristicas e acoes da classe animal. 
  - Entre a linha 30 a 31 estamos fazendo a chamada de metodos do objeto cachorro. na linha 30 estamos passando um parametro para o metodo formaDeAndar(forma: "andando"), ao contrario da linha 31, que so chamamos o metodo, entao sua saida sera o que esta definido na classe. 

  1. Os construtores são tipos especiais de métodos usados ​​para criar e inicializar objetos. É através deste tipo especial de método, que você cria instâncias de uma classe. Assim, os construtores permitem que o programador crie objetos da classe e defina valores padrão, limite a instanciação e grave códigos flexíveis e fáceis de ler[sintaxe abaixo]. 

  ![metodo construtor!](https://i.imgur.com/Ma8oUQA.png)

  2. Veja que na linha 10 utilizamos a palavra reservada [init], dentro dos parametros colocamos os atributos declarados na classe. Dentro do bloco do [init] colocamos a palavra reservada [self] para endicar que os valores dos atributos do objeto pertence aos atribustos da classe.
  ![codigo Completo do codigo com saida!](https://i.imgur.com/czujnES.png)

  ## herenca

  - Quando uma classe erda os atributos e metodos de uma classe pai (ou Super Classe). 
  - Sintaxe class Aluno : Pessoa{} -> 







  


  ---

## SwiftUI

### O que e um view?

- E um obejto que representa uma interface graficaara o usuario, podem ser armazenadas em variaveis, também possuem propriedades que podem ser configuradas para definir sua aparência e comportamento, como sua cor de fundo, tamanho, posição, alinhamento, etc.
  
  #### 🎳 Tipos de aliamentos de uma view

    - [Stack] e a palavra reservada para informar que se pode combinar, ordenar ou agrupar uma série de elementos de um conjunto de views enpilhadas. (OBS: uma Stack empilhar 10 subvisualizações, caso contrário, a mensagem “A argumento extra na chamada” será exibida no seu editor).
  
    - [VStack] Ordena um embaixo do outro.

    - [HStack] Oordena um do lado do outro.
  
    - [ZStack] - ordena um por cima do outro.

     ![Imagem sobre tipos de Stack](https://gorillalogic.com/wp-content/uploads/2021/07/image2-1.png)

  ## modificadores()

    - [.LazyVStack e .LazyHStack] e o conteudo e carregado de acordo com o scroll da tela, ao contraeio da Stack comum que o conteudo e carregado totalmente.
  
     - [.ScrollView()] Comando que permite o scroll da pagina.

     - [.padding()] Funcao que da espaco das margens

     - [.Spacer()] espacamento entre as view, se colocar embaixo a view sobe do contrario ela desce. Obs: preence um espaco vazio.

     - [.frame()] modificador de tamanho, dentro do () pode-se usar o Widht: , height: , aliement: , etc

     - 1[minwidht e maxwidht o mesmo para height] definem respectivamente espaco minimo a ser ocupado e espaco maximo

     - [height] = altura

     - [wight] = largura
    
    - [.foregroundColor(.cor)] muda a cor

     - [.background(Color(.blue))] muda a cor de fundo para azul

    - [.image] adiciona uma imagem
        - [.resizable()] permite a re escala da imagem ouc 

        - [.imageScale(.large)] modifica a escala da imagem

    - [.ignoreSafeArea()] ignora a safe area do iphone 

    - [.divider()] divide a tela, cria uma linha de acordo com o tipo de view
        - teste

    ### navegation View

    - Para navegar entre paginas e nescessario criar uma [NavigationView{}]

        - Dentro de uma VavigationView coloca-se [NavigationLink] dentro do codigo, coloca-se o nome da outra tela test().

        - [.navigationView("Titulo da pagina")] modificador de uma naviagationView que adiciona um titulo.

         ![navigationView](https://i.imgur.com/6472B2w.png)

      - [TabView] 


  ## Wrappers 

  - Link sobre Wrappers: https://levelup.gitconnected.com/state-vs-stateobject-vs-observedobject-vs-environmentobject-in-swiftui-81e2913d63f9
  - [@State] um tipo de wrapper de propriedade que pode ler e gravar um valor gerenciado pelo SwiftUI. O estado é a fonte de verdade mais simples que seu aplicativo pode ter. Ele foi projetado para conter tipos de valor simples, como Ints, Strings e Bools. Ele não foi projetado para tipos de referência mais complexos, como quaisquer classes ou structs que você mesmo define e usa em seu aplicativo. *@State* não é a solução certa para nada além do mais simples dado.

  - [@StateObeject] Um tipo de wrapper de propriedade que instancia um objeto observável complexo como classes, entretanto a classe deve ser do tipo :ObersableObeject. `Importante:` entrar em sua visão por meio de uma NavigationLink, modifique o valor, quando voltar para  NavigationView pai, em seguida, seu avlor sera reiniciado para o estado original. Na verdade sua classe sera reiniciada.

  ```
  classe TestObject: ObservableObject {
    @Published var num: Int = 0
  }
  ```
  - [@Published] E um Wrapper que informa sempre que as  propriedades dentro do objeto observável mudar, queremos que a visão seja renderizada novamente.


  - [Binding] monitora as mundancas de um estado de uma propriedade em outro lugar.

  - [Button] cria um butao Button("Nomre do butao"){
      //acao do butao
  }.buttonStyle(.borderedProminent) -> label pradao do butao

  - [TextField("mensagem", text: $texto)] funcao para receber os dados do usuario -> [.textFildStyle(.roundedBorder)] style padrao do cmpo do texto

 - [.sheet]

 - [Toggle("texto", isOn: $variavel)] interruptor de true e false 

 - [Slider(Value: $vaariavel), in: [range], step: @2.0] slider tipo volume

 ### inconsistencia de dados 

- E quando a informacoes inconcistentes que nao batemcom a realidade.
