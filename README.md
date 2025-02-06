class Time {
    constructor(nome) {
        this.nome = nome;
        this.capitao = null;
    }

    definirCapitao(jogador) {
        this.capitao = jogador;
        console.log(`${jogador} agora é o capitão do time ${this.nome}.`);
    }

    exibirCapitao() {
        if (this.capitao) {
            console.log(`O capitão do time ${this.nome} é ${this.capitao}.`);
        } else {
            console.log(`O time ${this.nome} ainda não tem um capitão definido.`);
        }
    }
}

// Exemplo de uso
const meuTime = new Time("Leões");
meuTime.exibirCapitao(); // Ainda não tem um capitão
meuTime.definirCapitao("Carlos"); // Define o capitão
meuTime.exibirCapitao(); // Exibe o capitão atual
