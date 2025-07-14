# EduFocusAI - Landing Page

## 📚 Sobre o Projeto

Landing page moderna para o EduFocusAI, uma plataforma de aprendizado personalizado para estudantes com TDAH. Desenvolvida com foco em design educacional, gamificação e acessibilidade.

## 🎨 Design System

- **Paleta de Cores**: Roxo educacional (#8B5CF6), Azul ciano (#06B6D4), Laranja (#F59E0B)
- **Tipografia**: Inter - legível e moderna
- **Componentes**: Botões arredondados, cards com sombras, badges gamificados
- **Responsividade**: Mobile-first design

## 🚀 Tecnologias Utilizadas

- HTML5 semântico
- CSS3 com Tailwind CSS
- JavaScript vanilla
- Design responsivo
- Elementos de gamificação

## 📊 Funcionalidades

- ✅ Design responsivo e acessível
- 🎯 Seção hero com vídeo de fundo
- 📈 Métricas visuais de impacto
- 🏆 Badges de progresso e conquistas
- 🎨 Componentes do design system educacional
- 📱 Otimizado para mobile

## 🌐 Deploy na Vercel

### Pré-requisitos
- Conta na [Vercel](https://vercel.com)
- Git instalado
- Repositório no GitHub

### Instruções de Deploy

1. **Clone o repositório**
   ```bash
   git clone <seu-repositorio>
   cd edufocus-landing-page
   ```

2. **Conecte com a Vercel**
   ```bash
   # Instale a CLI da Vercel
   npm i -g vercel

   # Faça login na Vercel
   vercel login

   # Deploy
   vercel
   ```

3. **Deploy automático**
   - Conecte o repositório GitHub à Vercel
   - Toda mudança na branch main será automaticamente deployada

### Configuração Personalizada

O arquivo `vercel.json` está configurado para:
- Servir o site como estático
- Redirecionar todas as rotas para index.html
- Headers de segurança incluídos
- Otimização automática de assets

## 📁 Estrutura do Projeto

```
edufocus-landing-page/
├── index.html          # Página principal
├── package.json        # Configuração do projeto
├── vercel.json         # Configuração da Vercel
├── README.md           # Documentação
└── .gitignore          # Arquivos ignorados
```

## 🎯 Otimizações Implementadas

- **Performance**: Assets otimizados, lazy loading
- **SEO**: Meta tags apropriadas, estrutura semântica
- **Acessibilidade**: Contraste adequado, foco visível
- **Segurança**: Headers de segurança configurados

## 🔧 Desenvolvimento Local

```bash
# Servir localmente
python -m http.server 3000

# Ou usar qualquer servidor HTTP
npx http-server .
```

## 📝 Licença

MIT License - veja o arquivo LICENSE para detalhes.

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

---

**EduFocusAI** - Transformando a educação através da tecnologia 🚀 