# 371.-Configura-o-do-Projeto-JAVA-FX_2
Botoe melhorados
INICIO
__________________________________________
package basico;

import javafx.application.Application;
import javafx.geometry.Pos;
import javafx.scene.Scene;
import javafx.scene.control.Button;
import javafx.scene.layout.HBox;
import javafx.stage.Stage;

public class PrimeiroFX extends Application{
	
	@Override
	public void start(Stage primaryStage) throws Exception {
		
		Button botaoA = new Button("A");
		Button botaoB = new Button("B");
		Button botaoC = new Button("C");
		
		botaoA.setOnAction(e -> System.out.println("Apertou tecla A!"));
		botaoB.setOnAction(e -> System.out.println("Apertou tecla B!"));
		botaoC.setOnAction(e -> System.exit(0)); //fecha aplicação
		
		HBox box = new HBox(20);
		box.setAlignment(Pos.CENTER);
		box.setSpacing(20);
		box.getChildren().add(botaoA);
		box.getChildren().add(botaoB);
		box.getChildren().add(botaoC);
		
		Scene unicaCena = new Scene(box, 200, 150);
		
		primaryStage.setScene(unicaCena);
		primaryStage.show();
	}
	public static void main(String[] args) {
		launch(args);
		
	}
}

![image](https://user-images.githubusercontent.com/95525963/152684241-604ae30a-4aeb-4dfc-a736-e296dffddd62.png)

