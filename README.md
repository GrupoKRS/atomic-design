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

- **Página** - Agrupamento de organismos adicionando o comportamento e a lógica de negócio.


## Divisão de pastas

- Átomos - Tipos (buttons, inputs, links, etc)

- Molécula - **A DEFINIR**

- Organismos - **A DEFINIR**

- Páginas - Separada pelo next (rota)

## Ideias

- Ter protótipo de baixa fidelidade para as páginas do sistema
