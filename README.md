    //NUMERO9
    enum pontocardeal: byte { norte, sul , leste, oeste};
    enum cor { azul , verde , amarelo, vermelho}//um EXpasse o mouse em cima daa palavras e veja seus
    enum opcoes { criar = 1, deletar, editar, listar, atualizar}//valores crescentes e alteraveis
    
    static void Main(string[] args)
    {
        pontocardeal direcao = pontocardeal.sul;
        Console.WriteLine((int)direcao);
        listapontos();
        /*//NUMERO ESPECIAL ENUMS
        Console.WriteLine("selecione uma delas por favor");
        Console.WriteLine("1-criar\n2-deletar\n3-editar\n4-lista\n5-atualizar");///n e quebra de linha
        int index = int.Parse(Console.ReadLine());
        opcoes opcaoselcionada = (opcoes)index;// o numero inteiro sera convertido para o conteudo de opcoes
        
        switch (opcaoselcionada)
        {
            case opcoes.criar:
                Console.WriteLine("iniciando criaçao...");
                break;
            case opcoes.deletar:
                Console.WriteLine("deletando arquivo...");
                break;
            case opcoes.editar:
                Console.WriteLine("abrindo editor studio...");
                break;
            default:
                Console.WriteLine("ouve uma falha no comando...");
                break;
        }
        */


        //NUMERO 1
        /*//verdadeiro ou falso?????
        string yes = "victor";  
            Console.Write(yes == "victor");
        Console.ReadLine();

        //NUMERO 2
        */
        /*//repetiçao
        for (int i = 0; i < 4; i++) 
        {
            Console.WriteLine("helloworld ");
            Console.ReadLine();
        }
        */

        //NUMERO 3
        /*// se senao e ou ????
        int a = 10, b = 30, c = 70;
        if (a > b || a > c)
        {
            Console.WriteLine("verdade");
        }
        else
        {
            Console.WriteLine("falso");
        }
        Console.ReadLine();
        */

        //NUMERO 4
        /*//verificador de idade
       int num = int.Parse(Console.ReadLine());
        if(num >= 0 && num <= 11)
        {
            Console.WriteLine("vc e uma criança!");
        }
        else if(num >= 12 && num <= 18)
        {
            Console.WriteLine("vc e um adolecente!");
        }
        else
        {
            Console.WriteLine("vc e um adulto");
        }
        Console.ReadLine();
        */

        //NUMERO 5
        /*// EXIBIR FUNÇAO 
        FUNCAO();
        FUNCAO();
        FUNCAO();
       */

        //NUMERO 6
        /*//outro exemplinho para voce sobre as funcoes
        calculo(70, "celular");
        calculo(150, "mochila");
        calculo(-99, "oxigenio");
        */

        //NUMERO 7
        /*
        carculo(80);
        carculo(54);
        carculo(-33);
        */

        /*//NUMERO 8
      int soma1 = somar(1,2, 3);
      int soma2 = somar(10, 20, 30);
      int soma3 = somar(100, 200, 300);
        Console.WriteLine(soma1);
        Console.WriteLine(soma2);
        Console.WriteLine(soma3);
        */

        /*//ARRAY
        int[] good = new int[3];
        good[2] = 300;
        Console.WriteLine(good[0]);
        Console.WriteLine(good[1]);
        Console.WriteLine(good[2]);
        */


        /* //CASO
         Console.WriteLine("digite uma cor ");
       string cor =  Console.ReadLine();
         switch (cor){
             case "vermelho":
                 Console.WriteLine("sua corzinha e vermelho");
                 break;
             case "verde":
                 Console.WriteLine("sua corzinha e verde");
                 break;
             case "preto":
                 Console.WriteLine("sua corzinha e preto");
                 break;
             default:
                 Console.WriteLine("hmmmm ok ");
                 break;
         }
         */
        //WHILE AND FOR ---> enquanto e para
        /*//DO WHILE
        do
        {
            Console.WriteLine("cu");

        } while (10000 < 14);
        */
        //FOREACH
        /*
        string[] palavras = { "oi", "tudo bem"," beleza"};
        foreach(string PALAVRA in palavras)//para cada PALAVRA no array de palavras repita o codigo
        {
            Console.WriteLine("yeeeees");
            Console.WriteLine(PALAVRA);
            //Console.WriteLine(palavras);//C# em mau funcionamento
        }
       for (int n1 = palavras.Length; n1 > 0; n1++)
        {
            
            Console.WriteLine(palavras[n1]);
            
        }
       */

        Console.ReadLine();
    }

    //CUIDADO FUNÇOES ABAIXO
    //o void significa que sua funçao naao retorna nada
    static void FUNCAO()
    {
        Console.WriteLine("1");
        Console.WriteLine("2");
        Console.WriteLine("3");
    }

    //CALCULO MERCADO V1
    static void calculo(int preco, string nome)
    {
        
        Console.WriteLine("o produto e " + nome);
        Console.WriteLine(preco + " o preço");  
    }

    //CALCULO MERCADO V2
    static void carculo(int PRECO){
        int PRECOABS = Math.Abs(PRECO);//garantia de que o preço sempre sera positivo
        int valorfinal = PRECOABS + (2 * PRECOABS);
        Console.WriteLine("valor final: " + valorfinal);
    }

    //SOMA e RETORNO
    static int somar(int a, int b, int c)
    {
        int resultadofinal = a + b + c;
        return resultadofinal;
    
    }
     static void listapontos()
 {
     pontocardeal ponto = pontocardeal.norte;
     for(int i = 0; i < 3; i++)
     {
         Console.WriteLine(ponto);
         ponto++;
     }
     Console.WriteLine(ponto);
     Console.ReadLine();
   }
}
