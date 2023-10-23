# DecIR
Exemplo GUI Declaração IR

Resumo:

A aplicação é uma interface gráfica (GUI) em Java que permite ao usuário inserir dados relacionados à declaração de imposto de renda. A GUI tem duas abas: "Identificação" e "Valores".

Na aba "Identificação", o usuário pode inserir seu nome e CPF. Na aba "Valores", o usuário pode inserir a renda anual e as deduções. Após inserir essas informações, o usuário pode pressionar o botão "Enviar", que calculará o imposto devido com base na fórmula :

(rendaAnual - deducoes) * 0.15. 

Após o cálculo, a aplicação cria um arquivo RTF contendo um resumo dos valores inseridos e do imposto calculado e tenta abrir esse arquivo para visualização.

import java.awt.Desktop;
import java.io.File;
import java.io.FileOutputStream;
import java.io.FileWriter;
import java.io.IOException;
import java.util.logging.Level;
import java.util.logging.Logger;
import javax.swing.JOptionPane;
import javax.swing.text.BadLocationException;
import javax.swing.text.Document;
import javax.swing.text.rtf.RTFEditorKit;
