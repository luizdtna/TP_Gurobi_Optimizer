Trabalho 1 da disciplina de Pesquisa Operacional.
Aluno: Luiz Araujo de Souza

#### Paços para instalação Gurobi no Linux Ubunto 20.0.4
* Baixar o Gurobi Optimizer
* Faça cadastro no Gurobi.com e gere sua licença educacional
* Colocá-lo na Pasta pessoal: /home/usuario/
* Abrir o terminal e descompactar o arquivo baixado:
	* tar xzvf gurobi9.1.0_linux64.tar.gz 
* Navegue até a pasta /home/luiz/gurobi910/linux64/src/build e execute o comando: 
	* make
* copie o arquivo libgurobi_c++.a da pasta /build para a pasta /gurobi910/linux64/lib 
* na pasta pessoal, aperte Ctrol+h e abra o arquivo .bashrc. Nele será incluído as seguintes linhas:

export GUROBI_HOME="/home/SEU_USUARIO/gurobi910/linux64"
export PATH="${GUROBI_HOME}/bin:${PATH}"
export LD_LIBRARY_PATH="${LD_LIBRARY_PATH}:${GUROBI_HOME}/lib"

* Execute sua licença do Gurobi. Para isso, vá até a o arquivo gurobi910/linux64/bin/grbgetkey e cole a licença

#### Após instalação do Gurobi, é possivel executar o trabalho

* Instale o __Jupyter Notebook__ em https://jupyter.org/install

* execute o comando __jupyter notebook__ no terminal. Você deve estar na pasta raiz deste projeto

* Será aberto uma aba em seu navegador, então selecione o arquivo TP1_Otimizacao_Gurobi.ipynb e execute em __Run__ os blocos de exercícios

