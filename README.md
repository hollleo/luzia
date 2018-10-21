# luzia
public class Livros {
	public static void main(String[] args) {
	int livro;
	int livroOpc;
	int opcBcktMn;
	int opcLoja;
	int opcLoja1;
	int opcMenu;
	int opcBcktMn1;
	Scanner entrada = new Scanner(System.in);
	int i=1;
	
	//MENU PRINCIPAL
	System.out.println("Bem vindo a Luzia!\n");
	while (i ==1) {
	
	System.out.println("1. Localizar Livros");
	System.out.println("2. Sugerir Livros\n");
	opcMenu = entrada.nextInt();
	if(opcMenu ==1) {
	System.out.println("Gêneros: \n");
	System.out.println("1. Romance");
	System.out.println("2. Politica");
	
	livro = entrada.nextInt();
	// SELECAO DE GENERO
	if(livro == 1) {
		System.out.println("Genero Selecionado: Romance\n" + "Romance: Corredor A\n"
	+ "Exemplares de Romance: \n" + "\n" + "1. Jane Austen\n" + "2. William Shakespeare\n");
		System.out.println("Selecione exemplar:");
	livroOpc = entrada.nextInt();
	
	if(livroOpc == 1) {
		System.out.println("Livros deste exemplar estão disponiveis nesta escola!\n");
		
	}
	//RECOMENDACAO DE LOJA
	if(livroOpc == 2) {
		System.out.println("Livros deste exemplar não estão disponíveis nesta escola");
		System.out.println("Deseja consultar em outras livrarias? \n" + "1. SIM      2. NÃO");
		opcLoja = entrada.nextInt(); 
		if(opcLoja == 1) {
			System.out.println("Livrarias disponíveis: \n" + "Saraiva: ");
			System.out.println("Deseja comprar o livro por esse site?\n" + "1. SIM     2. NÃO");
			opcLoja1 = entrada.nextInt();
			if(opcLoja1 == 2) {
	
			}else {
				//LINK DE QR CODE
				System.out.println("https://www.saraiva.com.br/");
			}
			
		}else {
			
		}
		}
	System.out.println("Deseja procurar outro genero? \n" + "1. SIM      2. NAO");
	opcBcktMn = entrada.nextInt();
	
	if(opcBcktMn == 2) {
		System.out.println("Obrigado, volte sempre!");
		break;
	}else {
		continue;
	}
		
	}
	if(livro==2) {
		System.out.println("Genero Selecionado: Politica\n" + "Politica: Corredor B\n"
				+ "Exemplares de Politica: \n" + "\n" + "1. Karl Marx\n" + "2. Antonio Gramsci\n");
					System.out.println("Selecione exemplar");
		livroOpc = entrada.nextInt();
					
					if(livroOpc == 1) {
						System.out.println("Livros deste exemplar estão disponiveis nesta escola!\n");
						System.out.println("Deseja consultar em outras livrarias? \n" + "1. SIM      2. NÃO");
						opcLoja = entrada.nextInt(); 
						if(opcLoja == 1) {
							System.out.println("Livrarias disponíveis: \n" + "Saraiva: ");
							System.out.println("Deseja comprar o livro por esse site?\n" + "1. SIM     2. NÃO");
							opcLoja1 = entrada.nextInt();
							if(opcLoja1 == 1) {
								//LINK DE QR CODE
								System.out.println("https://www.saraiva.com.br/\n");	
							}else {
								
							}
							
						}
						
					}
					
					if(livroOpc == 2) {
						System.out.println("Livros deste exemplar estão disponiveis nesta escola!\n");
					}
					System.out.println("Deseja procurar outro genero? \n" + "1. SIM      2. NAO");
					opcBcktMn = entrada.nextInt();
					
					if(opcBcktMn == 2) {
						System.out.println("Obrigado, volte sempre!");
						break;
					}else {
						continue;
					}
						
	

	
	}
	if(livro >2) {
		System.out.println("Opção inválida!!!");
		
	}
	
	}
	if(opcMenu == 2) {	
		String sugestao;
		System.out.println("Informe o nome do livro que deseja sugerir: ");
		sugestao = entrada.next();
		System.out.println(sugestao + " sugerido com sucesso!!!\n");
		
		System.out.println("Deseja voltar ao menu principal?\n" + "1. SIM             2. NÃO\n");
		opcBcktMn1 = entrada.nextInt();
		if(opcBcktMn1 == 2) {
			System.out.println("Obrigado, volte sempre!");
			
			}
		if(opcBcktMn1 >=3) {
			System.out.println("Opção inválida!");
		}else {
			continue;
		}
		
		
	}
	if(opcMenu >=3) {
		System.out.println("Opção inválida!!!");
		
			
	}
	break;
	}
	}
	}
