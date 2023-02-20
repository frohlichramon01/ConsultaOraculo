<h1>Consulta Automatizada de Oráculo</h1>
<br>
<h3>Script de Consulta automatizada de nomes no sistema Oráculo TJ/PR</h3>
<br>
<h3>Instalação</h3>
<ol>
    <li>Salve os arquivos numa pasta;</li>
    <li>Acesso o terminal/prompt de comando nesta pasta;</li>
    <li>Digite <strong>pip install -r requirements.txt</strong>;</li>
</ol>
<br>
<h3>Instruções de Uso</h3>

<h4>1. Credenciais:</h4>
<p>As credenciais de login devem ser escritas conforme o arquivo <strong>login.txt (que não deve ser renomeado)</strong>
    conforme abaixo:
<ul>
    <li><strong>CPF</strong> na primeira linha</li>
    <li><strong>SENHA</strong> na segunda linha</li>
</ul>
O arquivo fica armazenado localmente e não é disponibilizado à rede pelo script, por isso são necessários cuidados em
sua eventual exposição.
</p><br>

<h4>2. Nomes para Consulta:</h4>
<p>Os nomes devem ser colocados <strong>um em cada linha</strong> no arquivo <strong>nomes.txt (que não deve ser
        renomeado)</strong>, como constam no documento de exemplo.
<ul>
    <li>Os nomes constantes no arquivo deste respositório são apenas exemplos.</li>
</ul>
</p><br>

<h4>3. Utilização:</h4>
<p>Configurados os dados nos arquivos <strong>login.txt</strong> e <strong>nomes.txt</strong>, acesse o terminal/prompt
    de comando e execute o comando <strong>python Consulta.py</strong>.
</p><br>

<h4>4. Resultados:</h4>
<p>Os resultados serão planilhados num arquivo chamado <strong>"Consulta_Oraculo DATA e HORA.xlsx"</strong>, e exibidos
    conforme abaixo:</p>
<table>
    <thead>
        <th>Nome Consultado</th>
        <th>Resultado</th>
        <th>Data/Hora</th>
    </thead>
    <tr>
        <th>Nome 1</th>
        <th><strong>Limpo</strong></th>
        <th>Data/Hora da consulta 1</th>
    </tr>
    <tr>
        <th>Nome 2</th>
        <th><strong>Verificar
                <?strong></th>
        <th>Data/Hora da consulta 2</th>
    </tr>
    <tr>
        <th>...</th>
        <th>...</th>
        <th>...</th>
    </tr>
</table>

<p>Os resultados são classificados em:
<ul>
    <li><strong>LIMPO</strong></li>
        <ul><li>Significa que não houve nenhum resultado pela consulta simples do nome, mesmo sem a filiação.</li></ul>
    <li><strong>VERIFICAR</strong></li>
        <ul>
            <li>Significa que houve algum resultado para o nome, sem a filiação.</li>
            <li>Neste caso há necessidade de consulta manual, informando a filiação, para evitar resultados homônimos.</li>
        </ul>
</ul>
</p>

<h4>5. Observações:</h4>
<p>A análise do Oráculo depende de interpretação, por isso o script simplifica a consulta, evitando a consulta manual de cada indivíduo, já descartando quem não possui registro.</p>
