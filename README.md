# calculo-de-m-dia
não autoral

const estudantesTurmaA = [
    {
        nome: 'mateus',
        nota: 10
    },
    {
        nome: 'jorge',
        nota: 6.4
    },
    {
        nome: 'maria',
        nota: 5.8
    }
]
const estudantesTurmaB = [
    {
        nome: 'carlos',
        nota: 9.8
    },
    {
        nome: 'felipe',
        nota:  3.5
    },
    {
        nome: 'ana',
        nota: 6.7
    },
    {
        nome: 'joaquina',
        nota: 3.2
    },
]
function calculaMedia(aluno) {
    let soma = 0;
    for (let i = 0; i < aluno.length; i++) {
       soma = soma + aluno[i].nota
    }
    const media = soma / aluno.length
    return media
}

const resultado1 = calculaMedia(estudantesTurmaA)
const resultado2 = calculaMedia(estudantesTurmaB)

function retornodemensagem(media, turma) {
    if (media > 6) {
        console.log(`a media da ${turma} foi de ${media}. parabens`)
    }else{
        console.log(`a media da ${turma} foi menor que 5`)
    }
}
retornodemensagem (resultado1, 'Turma A')
retornodemensagem (resultado2, 'Turma B')
