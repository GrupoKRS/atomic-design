# Definições das adaptações feitas no padrão [Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/) que será utilizado nos projetos da Envoy

## Definição 

- **Átomo** - Elemento básico HTML que existe de forma independente ou quando separados, não são aproveitáveis. Um átomo sozinho não forma coesão visual.
```
	<a></a>
	<h1></h1>
	<input />
	<ul>
		<li>
	</ul>    
	<dl>
		<dd></dd>
	</dl>    
	<table>      
		<tbody>
			<tr>      
  				<td></td>
			</tr>
    	</tbody>
	</table>     
	<label></label>
```
      
- **Molécula** - Agrupamento de átomos ou elementos HTML não reutilizáveis que formam um elemento visual.
      
- **Organismos** - Agrupamentos de moléculas, átomos ou elementos HTML não reutilizáveis. Um organismo não pode conter outro organismo.

- **Template** - Agrupamento de organismos sem a lógica da aplicação (sem redux, requisição, funções de tratamento de estado e etc)

- **Página** - Mescla o template a lógica do negócio.


## Divisão de pastas

- Átomos - Tipos (buttons, inputs, links, etc)

- Molécula - Separados por página (PostInternal, Contact, Blog, Navbar). Para moléculas globais, incluir na pasta globals e categorizar por organismo. 

- Organismos - Separados por página (PostInternal, Contact, Blog, Navbar). Para organismos globais, incluir na pasta globals.

- Template - Separado pelo next (rota)

- Páginas - Separada pelo next (rota)

# Repositórios com testes do atomic design

- https://github.com/lBrunol/atomic-design-blog

- https://github.com/marcospedro97/atomic

- https://github.com/jpsant/atomic-design

## Ideias

- Ter protótipo de baixa fidelidade para as páginas do sistema

## Referências

https://bradfrost.com/blog/post/atomic-web-design/

https://dennisreimann.de/articles/atomic-design-is-messy.html

https://patternlab.io/demos/
