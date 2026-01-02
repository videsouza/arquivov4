# Template Institucional GOV.BR – Sistemas Internos

Este template foi estruturado para servir como **base oficial reutilizável** para sistemas internos de órgãos públicos, universidades e entidades da administração direta ou indireta, seguindo:

* Design System GOV.BR
* e-MAG (Modelo de Acessibilidade em Governo Eletrônico)
* WCAG 2.1 – Nível AA
* Boas práticas de HTML semântico e CSS institucional

---

## 1. Estrutura de Diretórios Recomendada

```
/template-govbr
 ├── index.html          # Página principal / dashboard
 ├── govbr.css           # Estilos institucionais
 ├── assets/
 │   ├── icons/          # Ícones SVG institucionais (opcional)
 │   └── img/            # Logotipos ou imagens institucionais
 └── README.md           # Documentação do template
```

---

## 2. Princípios do Template

### 2.1 Neutralidade institucional

* Não utiliza linguagem promocional
* Não hierarquiza serviços por relevância subjetiva
* Adequado para uso contínuo e prolongado

### 2.2 Acessibilidade nativa

* Navegação completa por teclado
* Foco visível em todos os elementos interativos
* Conteúdo não dependente exclusivamente de cor ou ícone
* Compatível com leitores de tela (NVDA, JAWS, VoiceOver)

### 2.3 Manutenibilidade

* CSS separado do HTML
* Variáveis de cor centralizadas (`:root`)
* Componentes reutilizáveis (`.service-card`, `.services-grid`)

---

## 3. Como reutilizar o template

### 3.1 Criar um novo sistema

1. Copie a pasta inteira do template
2. Renomeie o projeto conforme o sistema
3. Ajuste apenas:

   * Título da página (`<title>`)
   * Texto da barra institucional superior
   * Links e descrições dos cards

Nenhuma alteração estrutural é necessária.

### 3.2 Adicionar novos cards

Use sempre o padrão abaixo:

```html
<a href="pagina.html" class="service-card" aria-label="Acessar Nome do Serviço">
  <div class="card-icon">
    <i class="fas fa-icon" aria-hidden="true"></i>
  </div>
  <h3 class="card-title">Nome do Serviço</h3>
  <p class="card-desc">Descrição objetiva e institucional.</p>
  <span class="card-action">Acessar</span>
</a>
```

---

## 4. Padrões obrigatórios

### 4.1 Não remover

* `.skip-link`
* `<main role="main">`
* Atributos `aria-label`
* Estilo de foco visível

### 4.2 Não adicionar

* Badges promocionais ("Novo", "Popular")
* Animações excessivas
* Cores fora da paleta GOV.BR
* Conteúdo transmitido apenas por ícone

---

## 5. Validação e conformidade

Antes de publicar:

* Validar HTML em [https://validator.w3.org/](https://validator.w3.org/)
* Testar navegação apenas com teclado
* Testar contraste (mínimo AA)
* Testar com leitor de tela

---

## 6. Licenciamento e uso

Este template pode ser utilizado, adaptado e expandido livremente em:

* Órgãos públicos
* Universidades federais, estaduais e municipais
* Arquivos públicos e sistemas administrativos

Recomenda-se manter este README como documentação base do sistema.

---

**Template institucional pronto para produção e auditoria.**
