-------------------------------------Permiçãoe-------------------------------------

ls -lha: mostra os arquivos e diretorios presentes no diretorio atual junto de sua
repectivas informações, incluindo o tipo e permições

1.222.333.444

-----------------------------------------------
1: tipo

Ex: --Comum
    D-Diretoio
    L-Link simbolico
    B-Dispositivo de Bloco
    C-Dispositivo de Caractere
    S-Socket
-----------------------------------------------
RWX
2: permições do Dono do Aqruivo

3: Permições do Grupo Dono do Arquivo

4: Permições de Outros
_______________________________________________

RWX                    Valor

R = Read-Leitura     | R=4
W = Writ-Escrita     | W=2
X = Execute-Execução | X=1

Ex Permição: 761

-.RWX.RW_.X__
  7   6	  1

-= comun
7= R+W+X: 4+2+1
6= R+W: 4+2
1= X: 1  

-----------------------------------------------
Chmod: Modifica as permiçõe de um arquivo ou diretorio 

Chwon: Modifica o Usuario Dono e o Grupo Dono do arquivo

-R: Adiciona um efeito de recursividade na ação de um comando

a-All
u-Usuario Dono
g-Grupo Dono
o-Outros

Modo Ugoa: Chmod 1 2 3

Modo Octal: Chmod 4 3
1: Usuario/Grupo Dono/ Outros
2: Tipo de Operação
3: arquivo/diretorio
4: Permição RWX

Ex Modo Ugou: chmod g=wx arqTes.md

Ex Modo Octal: chmdo 744 arqTes.md

Ex Chwon usuario + Grupo : chwon user_1:grup_d arqTes.md

Ex Chwon Usuario Dono: chwon user_1 arqTes.md

Ex Chwon Grupo Dono: chwon :grup_d arqTes.md

-----------------------------------------------

Permições Especiais

chmod & RWX arquivo/diretorio

&: Permição Especial   
-----------------------------------------------

Permição	  Valor

1: stic bit	| T
2: sgid		| 2
3: suid		| 4

1: Qualquer deretorio com essa permição "T" ativa,
   tera toda e qualquer alteração do seu conteudo
   apenas restringida para ao Usuario Dono

2: Quando essa permição estiver em vigor em um diretorio
   ou arquivo, qualquer usuario tera as mesmas permições  
   do Usuario Dono 

3: Semelhante ao "2", mas voltado para os Grupos

Ex: chmod 2744 arqTes.md
_______________________________________________
