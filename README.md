# IMAGEDATASET_ML
Conjunto de dados para testes de aplicações de RP em imagens.

Foram coletadas um total de 3435 imagens, sendo elas pertecentes as seguintes categorias:

\begin{itemize}
    \item Frutas (102)
    \item Plantações (1322)
    \item Animais (1232)
    \item CAPTCHA (124)
    \item Faces Humanas (400)
    \item Pinturas (255)
\end{itemize}

Nem todas imagens coletadas foram utilizadas nos experimentos realizados, mas todas elas estão disponíveis no github\footnote{link github} com os devidos créditos quando se tem uma única origem de maior relevância. A seguir tem-se uma descrição de todos esses conjuntos de imagens.

\subsection{Conjunto de imagens de frutas} 
Foram coletadas um total de 102 imagens de frutas através de buscas na internet, as imagens estão divididas em 5 classes.

\begin{table}[h]
	\centering
	\caption{Conjunto de dados 1 - Frutas}
	\vspace{0.5cm}
	\begin{tabular}{r|lr}
		CLASSE & OBJETOS \\ % Note a separação de col. e a quebra de linhas
		\hline                               % para uma linha horizontal
		BANANA & 20 \\
		LARANJA &  20 \\
		LIMÃO & 20 \\
		MAÇA & 20 \\
		MORANGO & 22 \\
	    \hline
		TOTAL & 102 \\
	\end{tabular}
\end{table}

As imagens estão em diversas resoluções, com diferentes perspectivas de capturas e podem conter uma ou várias unidades de alguma fruta. Algumas possuem fundo composto apenas por uma única cor sólida.

\subsection{Conjunto de Imagens de Plantações}
Foram coletadas através de sites de busca na internet um total de 1322 imagens de plantações, dividas em 12 classes.

\begin{table}[h]
	\centering
	\caption{Conjunto de dados 2 - Plantações}
	\vspace{0.5cm}
	\begin{tabular}{r|lr}
		CLASSE & OBJETOS \\ % Note a separação de col. e a quebra de linhas
		\hline                               % para uma linha horizontal
		ALGODÃO & 109 \\
		ARROZ &  116 \\
		MILHO & 110 \\
		GIRASSOL & 101\\
		MANDIOCA & 100 \\
		CANAVIAL & 106 \\        % não é preciso quebrar a última linha
		MAMAO & 110 \\
		BANANA & 113 \\
		JABUTICABA & 111 \\
		ABACAXI & 117 \\
		TOMATE & 130 \\
		ALFACE & 110 \\
		\hline
		TOTAL & 1322
	\end{tabular}
\end{table}

As imagens estão em diversas resoluções e com diferentes perspectivas de captura. Algumas possuem grandes plantações (que podem ter frutos visíveis ou não), outras apenas uma única instância, e algumas (uma pequena parcela) apenas frutos provenientes da plantação. Uma pequena parcela das imagens contém fundo composto por apenas uma única cor sólida.

\subsection{Conjunto de Imagens de Animais}
Foram coletadas através de sites de busca na internet um total de 1232 imagens de animais, dividas em 11 classes.

\begin{table}[h]
	\centering
	\caption{Conjunto de dados 3 - Animais}
	\vspace{0.5cm}
	\begin{tabular}{r|lr}
		
		CLASSE & OBJETOS \\ % Note a separação de col. e a quebra de linhas
		\hline                               % para uma linha horizontal
		HOMEM & 110 \\
		MACACO &  116\\
		SERPENTE & 110 \\
		TUBARÃO & 111 \\
		CROCODILO & 110 \\        % não é preciso quebrar a última linha
		CAVALO & 115 \\
		ELEFANTE & 112 \\
		BEIJA-FLOR & 115 \\
		GATO & 113 \\
		GIRAFA & 110 \\
		AVESTRUZ & 111 \\
		\hline
		TOTAL & 1232
	\end{tabular}
\end{table}

As imagens estão em diversas resoluções e com diferentes perspectivas de captura, algumas possuem partes do animal, outras o animal inteiro. Uma pequena parcela das imagens contém fundo composto por apenas uma única cor sólida.


\subsection{Conjunto de Imagens de CAPTCHA}
Foram coletadas imagens através de sites que utilizam o \textbf{CAPTCHA} \textit{(Completely Automated Public Turing test to tell Computers and Humans Apart)} como medida de segurança contra ataques automatizados por máquinas. Para isso foram capturadas imagens de tais testes através da captura de tela e então separadas cada imagem envolvida, totalizando 124 imagens.

As imagens foram separadas em apenas 2 classes para simulação do teste de "Selecione Um Veículo", onde o objetivo é apenas classificar as imagens como contendo ou não veículos, as mesmas imagens poderiam ser organizadas em outros conjuntos binários (2 classes) para simular outros tipos de situações que ocorrem nesse teste.

\begin{table}[h]
	\centering
	\caption{Conjunto de dados 4 - CAPTCHA}
	\vspace{0.5cm}
	\begin{tabular}{r|lr}
		
		CLASSE & OBJETOS \\ % Note a separação de col. e a quebra de linhas
		\hline                               % para uma linha horizontal
		VÉICULOS & 54 \\
		NÃO\_VEÍCULOS & 70 \\ 
		\hline
		TOTAL & 124
	\end{tabular}
\end{table}

As imagens possuem resoluções similares com várias perspectivas de capturas e podem possuir apenas uma cor sólida, apenas um objeto ou uma grande variedade de objetos misturados na mesma imagem.


\subsection{Conjunto de Imagens de Faces Humanas - 'ORL Database Of Faces'}
\cite{orl_database}Esse conjunto de imagens, disponibilizado pela \textbf{Universidade de Cambridge}, chamado de \textit{'ORL Database of Faces'}, contém imagens da face de 40 indivíduos, sendo 10 imagens por indivíduo, totalizando 400 imagens.

\begin{table}[h]
	\centering
	\caption{Conjunto de dados 5 - 'ORL Database Of Faces'}
	\vspace{0.5cm}
	\begin{tabular}{r|lr}
		
		CLASSE & OBJETOS \\ % Note a separação de col. e a quebra de linhas
		\hline                               % para uma linha horizontal
		INDIVÍDUO0 & 10\\
		INDIVÍDUO1 & 10\\
		... & ...\\
	    INDIVÍDUO39 & 10 \\
		\hline
		TOTAL & 400
	\end{tabular}
\end{table}
\cite{orl_database}
Essas imagens foram capturadas entre 1992 e 1994 no Laboratório de Pesquisas Olivetti (ORL - Olivetti Research Laboratory) em Cambridge para testes de reconhecimento facial, estão todas dispostas na mesma resolução com a mesma perspectiva de captura. 

\textbf{Tradução e adaptação de um trecho informativo disponível junto ao conjunto de dados:} 

"Para alguns dos indivíduos, as suas 10 imagens foram capturadas em momentos diferentes, variando levemente a luz, expressões faciais e detalhes faciais. Todas as imagens foram tiradas em um fundo escuro homogêneo e todos os indivíduos estão encarando a câmera com possivelmente uma pequena variação de movimentos e inclinações laterais da cabeça."

Dados e informações disponíveis em:

\url{https://www.cl.cam.ac.uk/research/dtg/attarchive/facedatabase.html}


\subsection{Conjunto de Pinturas (Diferentes Movimentos Artísticos)}
Foram coletadas da enciclopédia de artes visuais, \textbf{WikiArt}\footnote{Endereço para acesso: \url{https://www.wikiart.org/} } imagens de pinturas de 6 movimentos artísticos, cada classe (movimento artístico) possui no mínimo 31 amostras e totalizam 255 imagens.

Foram utilizados movimentos de 3 eras diferentes:
\begin{itemize}
    \item Medieval(Pinturas dos movimentos Bizantino e Gótico);
    \item Pós Renascença (Pinturas dos movimentos Barroco e Romantismo);
    \item Moderna (Pinturas dos movimentos Cubismo e Expressionismo).
\end{itemize}

\begin{table}[h]
	\centering
	\caption{Conjunto de dados 7 - Movimentos Artísticos}
	\vspace{0.5cm}
	\begin{tabular}{r|lr}
		
		CLASSE & OBJETOS \\ % Note a separação de col. e a quebra de linhas
		\hline                               % para uma linha horizontal
		BIZANTINO & 37\\
		GOTICO & 31\\
		BARROCO & 49\\
		ROMANTISMO & 52\\
		CUBISMO & 43\\
		EXPRESSIONISMO & 43\\
		\hline
		TOTAL & 255
	\end{tabular}
\end{table}

As imagens variam bastante em resolução, e cada uma contém apenas uma pintura pertencente predominantemente a algum movimento artístico específico, podendo também exibir alguma características de outros movimento na mesma.
