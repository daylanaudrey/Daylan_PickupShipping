Versão utilizada: Magento 2.4.6 (compatível com qualquer versão da linha 2.4.x)

Processo para instalação tradicional via terminal:
1.	Mover o módulo para o diretório correto:
No terminal, acesse a raiz da instalação do Magento e mova o módulo para:
app/code/Daylan/PickupShipping/

Se estiver com o arquivo .zip, descompacte com:
unzip Daylan_PickupShipping.zip -d app/code/Daylan/PickupShipping

2.	Registrar o módulo no Magento:
Execute os seguintes comandos a partir da raiz do projeto:
php bin/magento setup:upgrade

3.	Recompilar o código (opcional, mas recomendado):
php bin/magento setup:di:compile

4.	Limpar o cache do Magento:
php bin/magento cache:flush

5.	Ativar o método de entrega no painel:
	Acesse o admin do Magento:
	•	Vá em: Lojas > Configuração > Vendas > Métodos de Entrega
	•	Localize “Retirado na Loja” (método pickupshipping)
	•	Ative o método e clique em “Salvar Configuração”
 
6.	Testar o método:
	•	No checkout da loja, a opção “Retirado na Loja” estará disponível como método de entrega gratuito
	•	No grid de pedidos no painel, o método aparece com suporte a filtro por método de envio
