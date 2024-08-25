# Classe para representar uma partida
class Partida:
    def __init__(self, id_partida, data_partida, nome_time, nome_adversario):
        self.id_partida = id_partida
        self.data_partida = data_partida
        self.nome_time = nome_time
        self.nome_adversario = nome_adversario

    def __str__(self):
        return (f"Partida(id_partida={self.id_partida}, data_partida='{self.data_partida}', "
                f"nome_time='{self.nome_time}', nome_adversario='{self.nome_adversario}')")


# Classe para representar um jogador
class Jogador:
    def __init__(self, nome_jogador, posicao, nome_time):
        self.nome_jogador = nome_jogador
        self.posicao = posicao
        self.nome_time = nome_time

    def __str__(self):
        return (f"Jogador(nome_jogador='{self.nome_jogador}', posicao='{self.posicao}', "
                f"nome_time='{self.nome_time}')")


# Classe para representar um resultado
class Resultado:
    def __init__(self, id_partida, nome_jogador, gols):
        self.id_partida = id_partida
        self.nome_jogador = nome_jogador
        self.gols = gols

    def __str__(self):
        return (f"Resultado(id_partida={self.id_partida}, nome_jogador='{self.nome_jogador}', "
                f"gols={self.gols})")


# Função principal para executar o código
def main():
    # Criar algumas instâncias de partidas
    partida1 = Partida(1, "2024-08-01", "Time A", "Time B")
    partida2 = Partida(2, "2024-08-02", "Time B", "Time C")

    # Criar alguns jogadores
    jogador1 = Jogador("João Silva", "Atacante", "Time A")
    jogador2 = Jogador("Pedro Santos", "Meio", "Time A")
    jogador3 = Jogador("Carlos Lima", "Defesa", "Time B")

    # Criar alguns resultados
    resultado1 = Resultado(1, "João Silva", 2)
    resultado2 = Resultado(1, "Pedro Santos", 0)
    resultado3 = Resultado(2, "Carlos Lima", 1)

    # Exibir as informações
    print(partida1)
    print(partida2)
    print(jogador1)
    print(jogador2)
    print(jogador3)
    print(resultado1)
    print(resultado2)
    print(resultado3)


if __name__ == "__main__":
    main()
