import javax.swing.JOptionPane;



public class Teste {

    public static void main(String[] args) {
   
        String Sim = null, sim = null, s = null;
        int resposta;
        int resposta1 = 0;
        int Animal;
       
        resposta = JOptionPane.showConfirmDialog(null, "Vamos cadastra animal hoje?");
        if (resposta == JOptionPane.YES_OPTION) {
            resposta1 = JOptionPane.showConfirmDialog(null, "Deseja cadastrar cachorro?");
                if (resposta1 == JOptionPane.YES_OPTION) {
                    Cachorro c1 = new Cachorro();
                    c1.nome = JOptionPane.showInputDialog("Qual o nome do cão?");
                    c1.idade = JOptionPane.showInputDialog("Qual a idade do cão?");
                    c1.raca = JOptionPane.showInputDialog("Qual é a raça do cão?");
                    c1.sexo = JOptionPane.showInputDialog("Qual o sexo do cão?");
                    c1.racao = JOptionPane.showInputDialog("Qual o ração do cão?");
                    c1.peso = JOptionPane.showInputDialog("Qual o peso do cão?");
                }if(resposta1 ==JOptionPane.showConfirmDialog(null, "Deseja cadastra gato?")) {
                    JOptionPane.showMessageDialog(null, "Deseja continuar?");
                    if (resposta1 == JOptionPane.YES_OPTION) {
                        Gato g1 = new Gato();
                        g1.nome = JOptionPane.showInputDialog("Qual o nome do gato?");
                        g1.idade = JOptionPane.showInputDialog("Qual o nome do gato?");
                        g1.raca = JOptionPane.showInputDialog("Qual o nome do gato?");
                        g1.sexo = JOptionPane.showInputDialog("Qual o nome do gato?");
                    }
                } else {
            JOptionPane.showMessageDialog(null, "Deseja continuar?");
        }
       
        }
    }
}




_______________________________________________________________________________________________________________________




public class Animal extends Rotina{
	
	String nome;
	String idade;
	String raca;
	String sexo;
	
	Rotina[] rotina;

}


____________________________________________________________________________


public class Cachorro extends Animal {
	
	Rotina[] cortePelo;
	

}


_____________________________________________________________________



public class Gato extends Animal {

}





________________________________________________



public class Rotina {
	
	String racao;
	String peso;
	

}
