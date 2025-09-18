# 🏪 CasaOS Tailscale AppStore

App Store personalizado para CasaOS com aplicações relacionadas ao Tailscale e ferramentas de rede segura.

## 🚀 Como Adicionar ao CasaOS

### Método 1: Interface Web (Recomendado)

1. **Abra o CasaOS Dashboard**
2. **Acesse a App Store**
3. **Clique em "Add Source" (canto superior direito)**
4. **Cole esta URL:**
   ```
   https://raw.githubusercontent.com/WillianQuintino/casaos-tailscale-appstore/main
   ```
5. **Clique em "Add"**

### Método 2: CLI

```bash
casaos-cli app-management register app-store https://raw.githubusercontent.com/WillianQuintino/casaos-tailscale-appstore/main
```

## 📱 Aplicações Disponíveis

### 🌐 Tailscale Funnel Manager
- **Categoria:** Network
- **Função:** Interface web para gerenciar Tailscale Funnels
- **Repositório:** [tailscale-funnel-manager](https://github.com/WillianQuintino/tailscale-funnel-manager)

**Funcionalidades:**
- ✅ Descoberta automática de containers CasaOS
- ✅ Criação de funnels com um clique
- ✅ Monitoramento em tempo real
- ✅ Interface web moderna e responsiva
- ✅ Suporte multi-idioma (EN/PT)

## 🔧 Requisitos

- **CasaOS:** Versão 0.4.4 ou superior
- **Docker:** Versão 20.10 ou superior
- **Arquiteturas:** AMD64, ARM64

## 📊 Informações do Store

| Item | Valor |
|------|-------|
| **Total de Apps** | 1 |
| **Categorias** | Network |
| **Idiomas** | Inglês, Português |
| **Última Atualização** | 2024-09-18 |

## 🛠️ Contribuir

Para adicionar novas aplicações a este app store:

1. **Fork este repositório**
2. **Adicione sua aplicação em `Apps/[CATEGORIA]/[NOME-APP]/`**
3. **Atualize os metadados:**
   - `featured-apps.json` (se destacada)
   - `recommend-list.json` (se recomendada)
   - `store.json` (contador de apps)
4. **Teste no seu CasaOS**
5. **Submeta Pull Request**

### Formato do Manifesto

```yaml
name: nome-da-aplicacao
services:
  service-name:
    image: namespace/image:tag
    # ... configuração Docker

x-casaos:
  architectures: [amd64, arm64]
  main: service-name
  author: Seu Nome
  category: Categoria
  description:
    en: English description
    pt: Descrição em português
  # ... outros metadados CasaOS
```

## 🔗 Links Relacionados

- **Projeto Principal:** [Tailscale Funnel Manager](https://github.com/WillianQuintino/tailscale-funnel-manager)
- **CasaOS:** [Documentação Oficial](https://casaos.zimaspace.com)
- **Tailscale:** [Site Oficial](https://tailscale.com)

## 🆘 Suporte

- **Issues:** [GitHub Issues](https://github.com/WillianQuintino/casaos-tailscale-appstore/issues)
- **Discussões:** [GitHub Discussions](https://github.com/WillianQuintino/casaos-tailscale-appstore/discussions)

## 📄 Licença

Este projeto está licenciado sob a Licença MIT.

---

**🏠 Mantido pela Comunidade CasaOS**