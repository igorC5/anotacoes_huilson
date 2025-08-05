# anotacoes_huilson

05/08/2025
REVISÃO

levar = []

ATIVIDADE 2:

se (promocoes.encontra("saco15pregos")) então {
    levar.add("saco15pregos");
    levar.add("saco15pregos");
} senão {
    levar.add("saco30pregos");
}
se (promocoes.encontra("serrote")) então {
    levar.add("serrote");
};

ATIVIDADE 3:

saldo = 30
almocou = false

verificaSaldo(valorUltimaTransacao) {
    se (saldo < 0) entao {
        saldo += valorUltimaTransacao 
        // como se não tivesse feito a ultima transacao
    }
}

se (acordaTarde) entao {
    saldo -= 5; // café no posto
    verificaSaldo(5)
}

saldo -= 15 // frete das compsaldos

se (saldo >= 20) entao {
    saldo -= 20 // bom almoco
    verificaSaldo(20)
    almocou = true
} senao {
    saldo -= 5 // pastel
}

se (saldo > 100 || saldo <= 20) entao {
    saldo += 50
    verificaSaldo(50)
} senao {
    saldo += 10
    verificaSaldo(10)
}

se (saldo > 40) {
    saldo -= 40
    verificaSaldo(40)
}

