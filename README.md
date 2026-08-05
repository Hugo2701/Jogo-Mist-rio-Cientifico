# Jogo-Mist-rio-Cientifico
Jogo para alunos do ensino médio sobre química e física
export default function JogoMisterioCientifico() {
  const trilhasPedagogicas = {
    '1aSerieEM': {
      fisica: ['Grandezas físicas', 'Movimento uniforme', 'Leis de Newton', 'Energia'],
      quimica: ['Modelos atômicos', 'Tabela periódica', 'Ligações químicas', 'Transformações químicas']
    },
    '2aSerieEM': {
      fisica: ['Termologia', 'Óptica', 'Ondulatória'],
      quimica: ['Soluções', 'Cinética química', 'Termoquímica', 'Funções inorgânicas']
    },
    '3aSerieEM': {
      fisica: ['Eletrostática', 'Eletrodinâmica', 'Circuitos elétricos'],
      quimica: ['Eletroquímica', 'Equilíbrio químico', 'Química orgânica']
    }
  };
  const campanha = {
    titulo: 'Operação Quantum San Diego',
    capitulos: [
      {
        nome: 'Capítulo 1 - Química Investigativa',
        cidades: ['Santos', 'Cubatão', 'Campinas'],
        habilidades: ['Tabela Periódica', 'Ligações Químicas', 'Cinética Química']
      },
      {
        nome: 'Capítulo 2 - Óptica Forense',
        cidades: ['Campinas', 'Sorocaba'],
        habilidades: ['Reflexão', 'Refração', 'Lentes']
      },
      {
        nome: 'Capítulo 3 - Mecânica e Movimento',
        cidades: ['São José dos Campos', 'Taubaté'],
        habilidades: ['Leis de Newton', 'Forças', 'Energia']
      },
      {
        nome: 'Capítulo 4 - Termologia Criminal',
        cidades: ['Ribeirão Preto', 'Araraquara'],
        habilidades: ['Calor', 'Temperatura', 'Dilatação']
      },
      {
        nome: 'Capítulo 5 - Eletricidade e Captura Final',
        cidades: ['São Paulo'],
        habilidades: ['Lei de Ohm', 'Circuitos Elétricos', 'Potência Elétrica']
      }
    ]
  };
  const bancoMissoes = [
    'Identificar substância a partir da reação química.',
    'Decifrar mensagem usando espectro luminoso.',
    'Calcular aceleração de veículo suspeito.',
    'Analisar circuito de segurança.',
    'Determinar concentração de solução encontrada na cena do crime.',
    'Resolver desafio de termoquímica para abrir um cofre.',
    'Comparar evidências usando densidade e massa específica.',
    'Investigar pilhas clandestinas usando eletroquímica.',
    'Reconstruir trajetória de laser em laboratório.',
    'Localizar criminoso usando princípios de ondas.'
  ];
  const relatorioProfessor = {
    competencias: [
      'Resolução de problemas',
      'Investigação científica',
      'Análise de evidências',
      'Argumentação científica',
      'Modelagem matemática'
    ],
    indicadores: [
      'Acertos por tema',
      'Tempo por missão',
      'Número de tentativas',
      'Capítulos concluídos',
      'Conquistas obtidas'
    ]
  };
  return (
    <div className='p-6'>
      <h1>🔎 Mistério Científico SP: Operação Quantum San Diego</h1>
      <h2>📚 Trilhas Pedagógicas</h2>
      <pre>{JSON.stringify(trilhasPedagogicas, null, 2)}</pre>
      <h2>🗺️ Campanha Completa</h2>
      <pre>{JSON.stringify(campanha, null, 2)}</pre>
      <h2>�� Banco de Missões</h2>
      {bancoMissoes.map((m,i)=><div key={i}>• {m}</div>)}
      <h2>📊 Relatório do Professor</h2>
      <pre>{JSON.stringify(relatorioProfessor, null, 2)}</pre>

      <h2>🏫 Aplicação Pedagógica</h2>      <ul>
        <li>Aprendizagem baseada em problemas.</li>
        <li>Gamificação alinhada ao Currículo Paulista.</li>
        <li>Avaliação diagnóstica e formativa.</li>
        <li>Integração entre Física, Química e investigação científica.</li>        <li>Trabalho colaborativo em equipes de detetives.</li>      </ul>
    </div>
  );
}
