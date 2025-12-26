<b>O job desenvolvido no Talend</b> tem como objetivo realizar a leitura, o tratamento e a geração de arquivos de dados (ETL), garantindo que todas as etapas ocorram de forma controlada e sem erros.

Foi gerado dados fíticios relacionados a pessoas (id, nome, sobrenome, data de nascimento) e seus endereços (Estados Unidos) como:(id_pessoa, endereço, número, estado, cidade).

Funcionamento do Job

Inicialmente, o job executa uma etapa de verificação (PreJob), na qual confere se os arquivos e diretórios necessários para a execução existem. Caso algum recurso obrigatório não esteja disponível, o job é interrompido, evitando falhas no processamento.

Em seguida, o job realiza a leitura de dois arquivos de entrada, no formato CSV, que contêm os dados brutos a serem processados. Os dados são enviados para um componente de transformação (tMap), onde ocorre a organização e o tratamento das informações. Onde são definidos quais campos serão utilizados, ajustes de valores e a estrutura final dos dados.

Após o tratamento, o fluxo de dados é dividido em dois caminhos distintos. Um deles é responsável pela geração de um arquivo CSV (relacionado aos erros, Ids nulos), enquanto o outro gera um arquivo no formato JSON (registros corretos).
<p></p>
<img width="1292" height="688" alt="image" src="https://github.com/user-attachments/assets/547cfe66-85f5-404e-8bad-bdbca8ff02d5" />
<p></p>

<b>Além disso, o job realiza uma amostragem dos dados processados</b>, exibindo os 5 primeiros registros para conferência, de forma a confirmar que o processo foi realizado com sucesso.
<p></p>
<img width="1311" height="630" alt="image" src="https://github.com/user-attachments/assets/af15e217-2b59-49b5-969e-947ce6492157" />

<p></p>


<b>O principal objetivo deste job é</b> automatizar o processamento de dados, garantindo:

Organização e padronização das informações;

Geração de arquivos em formatos diferentes;

Redução de erros manuais;

Maior controle e confiabilidade no processamento.
