# 🚌 LocalWab - Sistema de Rastreamento de Transportes Públicos

## Sobre o Projeto

LocalWab é um aplicativo web progressivo (PWA) desenvolvido para rastrear transportes públicos em tempo real nas estradas nacionais de Angola. O sistema permite que usuários localizem os dois transportes públicos mais próximos de sua localização atual.

## ✨ Funcionalidades Principais

### 1. **Rastreamento em Tempo Real**
- Localização GPS do usuário
- Identificação dos 2 transportes públicos mais próximos
- Atualização automática da posição dos transportes a cada 5 segundos
- Visualização em mapa interativo com rotas

### 2. **Sistema de Pagamento**
- Pagamento de 10 Kz via Multicaixa Express
- Ativação de rastreamento por 10 minutos
- Transferência bancária instantânea
- Interface de confirmação de pagamento

### 3. **Timer de Sessão**
- Contador regressivo de 10 minutos
- Reinicialização automática após término
- Visualização clara do tempo restante

### 4. **Informações Detalhadas**
- Distância até cada transporte (em km)
- Tempo estimado de chegada (em minutos)
- Velocidade atual do transporte (em km/h)
- Rota e nome do transporte

### 5. **Modo Offline/Online**
- Funciona mesmo sem conexão à internet
- Cache de recursos para acesso offline
- Indicador de status de conexão
- Service Worker para PWA

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura do aplicativo
- **CSS3** - Estilização moderna e responsiva
- **JavaScript (ES6+)** - Lógica do aplicativo
- **Leaflet.js** - Mapas interativos
- **Service Worker** - Funcionalidade offline
- **Geolocation API** - Localização do usuário

## 📱 Compatibilidade

- ✅ Navegadores modernos (Chrome, Firefox, Safari, Edge)
- ✅ Dispositivos móveis (iOS e Android)
- ✅ Tablets e desktops
- ✅ Funciona offline após primeira carga

## 🚀 Como Usar

### Instalação Local

1. Abra o arquivo `index.html` em um navegador web moderno
2. Permita o acesso à sua localização quando solicitado
3. O aplicativo carregará e mostrará sua posição no mapa

### Uso do Sistema

1. **Visualizar Localização**: O mapa mostrará sua posição atual em Luanda
2. **Ativar Rastreamento**: Clique em "Pagar 10 Kz via Multicaixa Express"
3. **Confirmar Pagamento**: O modal confirmará o pagamento
4. **Ver Transportes**: Os 2 transportes mais próximos aparecerão no mapa
5. **Acompanhar**: Timer mostrará tempo restante (10 minutos)
6. **Renovar**: Após 10 minutos, o sistema reinicia automaticamente

## 📊 Estrutura de Arquivos

```
localwab/
│
├── index.html          # Página principal do aplicativo
├── app.js              # Lógica JavaScript
├── service-worker.js   # Service Worker para PWA
└── README.md           # Este arquivo
```

## 🔧 Implementação em Produção

Para implementar o LocalWab em produção, você precisará:

### 1. **Backend/API**
- Servidor Node.js ou Python (Flask/Django)
- Banco de dados (PostgreSQL/MongoDB)
- API REST para comunicação
- WebSocket para atualizações em tempo real

### 2. **Integração GPS Real**
- Dispositivos GPS nos transportes públicos
- API para receber dados de localização
- Sistema de gerenciamento de frotas

### 3. **Sistema de Pagamento**
- Integração oficial com Multicaixa Express API
- Endpoint: `https://api.multicaixa.ao/`
- Credenciais merchant
- Certificados SSL/TLS
- Webhook para confirmação de pagamento
- Integração bancária para transferências

### 4. **Infraestrutura**
- Servidor cloud (AWS, Google Cloud, Azure)
- CDN para distribuição de conteúdo
- SSL/HTTPS obrigatório
- Balanceamento de carga

### 5. **Aplicativo Móvel Nativo**
- React Native ou Flutter
- Publicação na Google Play Store
- Publicação na Apple App Store
- Push notifications

## 🔐 Segurança

- HTTPS obrigatório para geolocalização
- Tokens JWT para autenticação
- Criptografia de dados sensíveis
- Validação de pagamentos no servidor
- Rate limiting para API

## 💰 Integração Multicaixa Express

### Documentação Necessária
Para integrar o Multicaixa Express, você precisará:

1. **Conta Merchant** no Multicaixa
2. **API Keys** fornecidas pelo Multicaixa
3. **Webhook URL** para callbacks de pagamento
4. **Conta Bancária** para receber transferências

### Fluxo de Pagamento
```javascript
1. Usuário clica em "Pagar"
2. App envia requisição para API Multicaixa
3. Multicaixa processa pagamento
4. Webhook confirma pagamento
5. Sistema ativa rastreamento
6. Transferência bancária é processada
```

## 🗺️ Dados de Transportes

Atualmente o aplicativo usa dados simulados. Para produção:

1. **Parceria com Operadoras**: Acordos com empresas de transporte
2. **Instalação de GPS**: Dispositivos em cada transporte
3. **API de Dados**: Sistema para coletar e distribuir dados
4. **Atualização em Tempo Real**: WebSocket ou polling

## 📈 Próximos Passos

### Funcionalidades Futuras
- [ ] Histórico de viagens
- [ ] Rotas favoritas
- [ ] Notificações push
- [ ] Avaliação de transportes
- [ ] Compartilhamento de localização
- [ ] Previsão de chegada com IA
- [ ] Integração com outros meios de pagamento
- [ ] Sistema de fidelidade/pontos
- [ ] Chat com motorista
- [ ] Reserva de lugares

### Melhorias Técnicas
- [ ] Otimização de performance
- [ ] Testes automatizados
- [ ] CI/CD pipeline
- [ ] Monitoramento e analytics
- [ ] Logs centralizados
- [ ] Backup automático

## 📞 Suporte

Para implementação completa do sistema, você precisará:

1. **Desenvolvedores Full-Stack**: 2-3 pessoas
2. **Designer UI/UX**: 1 pessoa
3. **Especialista em Pagamentos**: Integração Multicaixa
4. **DevOps**: Infraestrutura e deployment
5. **Tempo Estimado**: 3-6 meses para MVP

## 💡 Modelo de Negócio

- **Receita por Transação**: 10 Kz por consulta de 10 minutos
- **Volume Esperado**: Depende da adoção
- **Custos**: Infraestrutura + Desenvolvimento + Marketing
- **Parcerias**: Operadoras de transporte (comissão?)

## 📄 Licença

Este protótipo foi desenvolvido como demonstração de conceito.

## 🎯 Conclusão

O LocalWab é uma solução inovadora para o transporte público em Angola. Este protótipo demonstra todas as funcionalidades principais e pode ser expandido para um sistema completo de produção com as integrações necessárias.

**Desenvolvido com ❤️ para Angola**

---

**Nota**: Este é um protótipo demonstrativo. Para colocar em produção, são necessárias as integrações descritas neste documento, especialmente com o Multicaixa Express e sistemas GPS reais dos transportes públicos.