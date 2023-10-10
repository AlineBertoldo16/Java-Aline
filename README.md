Evento do botão da interace gráfica GUI

private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        try {
            double valor = Double.parseDouble(jTextField1.getText());
            double desconto = Double.parseDouble(jTextField2.getText());

            double resultado = valor * (1 - (desconto / 100));

            jLabel3.setText("Valor após o desconto: " + resultado);
        } catch (NumberFormatException e) {
            JOptionPane.showMessageDialog(this, "Entre com valores válidos.", "Erro", JOptionPane.ERROR_MESSAGE);
        }        // TODO add your handling code here:
    }    
