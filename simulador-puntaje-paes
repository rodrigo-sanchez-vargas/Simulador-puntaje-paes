import matplotlib.pyplot as plt

print("""Ponderador puntaje PAES admisión 2027
Carrera: Ingeniería Civil en Computación e Informática o afín.
Opciones disponibles:
            1. Ingeniería Civil de Computación - Pontificia Universidad Catolica de chile
            2. Ingeniería Civil en Computación - Universidad de Chile
            3. Ingeniería Civil en Informática - Universidad de Santiago de Chile
            4. Ingeniería Civil Informática - Universidad Federico Santa Maria
            5. Ingeniería Civil Informática - Universidad de Concepción
            6. Ingeniería Civil en Informática y Telecomunicaciones - Universidad Diego Portales
""")

while True:
    try:
        opcion = int(input("Ingrese el número de la carrera de interes: "))

        nem = int(input("Ingrese su puntaje NEM: "))
        ranking = int(input("Ingrese su puntaje Ranking: "))
        competencia_lectora = int(input("Ingrese su puntaje Competencia Lectora: "))
        matematicas_1 = int(input("Ingrese su puntaje Matemática 1: "))
        matematicas_2 = int(input("Ingrese su puntaje Matemática 2: "))
        ciencias = int(input("Ingrese su puntaje Ciencias: "))
        historia = int(input("Ingrese su puntaje Historia y Ciencias Sociales: "))
        break

    except ValueError:
        print("Por favor, ingrese un número válido.")


def uc(notas, rank, c_lectora, m_1, m_2, ciencia):
    return (
        (notas * 0.20)
        + (rank * 0.20)
        + (c_lectora * 0.10)
        + (m_1 * 0.20)
        + (m_2 * 0.15)
        + (ciencia * 0.15)
    )


def uchile(notas, rank, c_lectora, m_1, m_2, ciencia):
    return (
        (notas * 0.10)
        + (rank * 0.25)
        + (c_lectora * 0.10)
        + (m_1 * 0.20)
        + (m_2 * 0.20)
        + (ciencia * 0.15)
    )


def usach(notas, rank, c_lectora, m_1, m_2, ciencia):
    return (
        (notas * 0.25)
        + (rank * 0.25)
        + (m_1 * 0.10)
        + (m_2 * 0.15)
        + (c_lectora * 0.15)
        + (ciencia * 0.10)
    )


def usm(notas, rank, c_lectora, m_1, m_2, ciencia, history):
    if ciencia > history:
        mejor_prueba = ciencia
    else:
        mejor_prueba = history
    return (
        (notas * 0.15)
        + (rank * 0.20)
        + (c_lectora * 0.10)
        + (m_1 * 0.35)
        + (m_2 * 0.10)
        + (mejor_prueba * 0.10)
    )


def udec(notas, rank, c_lectora, m_1, m_2, ciencia):
    return (
        (notas * 0.20)
        + (rank * 0.15)
        + (m_1 * 0.25)
        + (m_2 * 0.15)
        + (c_lectora * 0.15)
        + (ciencia * 0.10)
    )


def udp(notas, rank, c_lectora, m_1, m_2, ciencia, history):
    if ciencia > history:
        mejor_prueba = ciencia
    else:
        mejor_prueba = history
    return (
        (notas * 0.10)
        + (rank * 0.30)
        + (c_lectora * 0.10)
        + (m_1 * 0.35)
        + (m_2 * 0.05)
        + (mejor_prueba * 0.10)
    )


if opcion == 1:
    puntaje_uc = uc(
        nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias
    )
    print(
        f"Puntaje ponderado en la Pontificia Universidad Católica de Chile es: {puntaje_uc:.2f}"
    )

    plt.figure(facecolor="#e9e0e0")
    plt.subplot(2, 1, 1)
    plt.bar(
        [
            "NEM",
            "Ranking",
            "CL",
            "M1",
            "M2",
            "Ciencias",
        ],
        [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias],
        color="blue",
    )
    plt.title("Puntajes PAES")
    plt.ylim(100, 1000)
    plt.tight_layout()

    plt.subplot(2, 1, 2)
    plt.bar(
        ["Puntaje ponderado", "Puntaje de corte"],
        [puntaje_uc, 898.10],
        color="blue",
        label=[f"Puntaje ponderado: {puntaje_uc:.2f}", "Puntaje de corte: 898.10"],
    )
    plt.title("Ingeniería Civil de Computación")
    plt.ylim(100, 1000)
    plt.tight_layout()
    plt.legend(loc="upper right")

    plt.show()

elif opcion == 2:
    puntaje_uchile = uchile(
        nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias
    )
    print(f"Puntaje ponderado en la Universidad de Chile es: {puntaje_uchile:.2f}")

    plt.figure(facecolor="#e9e0e0")
    plt.subplot(2, 1, 1)
    plt.bar(
        [
            "NEM",
            "Ranking",
            "CL",
            "M1",
            "M2",
            "Ciencias",
        ],
        [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias],
        color="blue",
    )
    plt.title("Puntajes PAES")
    plt.ylim(100, 1000)
    plt.tight_layout()

    plt.subplot(2, 1, 2)
    plt.bar(
        ["Puntaje ponderado", "Puntaje de corte"],
        [puntaje_uchile, 833.85],
        color="blue",
        label=[f"Puntaje ponderado: {puntaje_uchile:.2f}", "Puntaje de corte: 833.85"],
    )
    plt.title("Ingeniería Civil en Computación")
    plt.ylim(100, 1000)
    plt.tight_layout()
    plt.legend(loc="upper right")

    plt.show()

elif opcion == 3:
    puntaje_usach = usach(
        nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias
    )
    print(
        f"Puntaje ponderado en la Universidad de Santiago de Chile es: {puntaje_usach:.2f}"
    )

    plt.figure(facecolor="#e9e0e0")
    plt.subplot(2, 1, 1)
    plt.bar(
        [
            "NEM",
            "Ranking",
            "CL",
            "M1",
            "M2",
            "Ciencias",
        ],
        [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias],
        color="blue",
    )
    plt.title("Puntajes PAES")
    plt.ylim(100, 1000)
    plt.tight_layout()

    plt.subplot(2, 1, 2)
    plt.bar(
        ["Puntaje ponderado", "Puntaje de corte"],
        [puntaje_usach, 787.6],
        color="blue",
        label=[f"Puntaje ponderado: {puntaje_usach:.2f}", "Puntaje de corte: 787.6"],
    )
    plt.title("Ingeniería Civil en Informática")
    plt.ylim(100, 1000)
    plt.tight_layout()
    plt.legend(loc="upper right")

    plt.show()

elif opcion == 4:
    puntaje_usm = usm(
        nem,
        ranking,
        competencia_lectora,
        matematicas_1,
        matematicas_2,
        ciencias,
        historia,
    )
    print(
        f"Puntaje ponderado en la Universidad Federico Santa María es: {puntaje_usm:.2f}"
    )

    if ciencias > historia:
        plt.figure(facecolor="#e9e0e0")
        plt.subplot(2, 1, 1)
        plt.bar(
            [
                "NEM",
                "Ranking",
                "CL",
                "M1",
                "M2",
                "Ciencias",
            ],
            [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias],
            color="blue",
        )
        plt.title("Puntajes PAES")
        plt.ylim(100, 1000)
        plt.tight_layout()
    else:
        plt.figure(facecolor="#e9e0e0")
        plt.subplot(2, 1, 1)
        plt.bar(
            [
                "NEM",
                "Ranking",
                "CL",
                "M1",
                "M2",
                "Historia",
            ],
            [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, historia],
            color="blue",
        )
        plt.title("Puntajes PAES")
        plt.ylim(100, 1000)
        plt.tight_layout()

    plt.subplot(2, 1, 2)
    plt.bar(
        ["Puntaje ponderado", "Puntaje de corte"],
        [puntaje_usm, 820.05],
        color="blue",
        label=[f"Puntaje ponderado: {puntaje_usm:.2f}", "Puntaje de corte: 820.05"],
    )
    plt.title("Ingeniería Civil Informática")
    plt.ylim(100, 1000)
    plt.tight_layout()
    plt.legend(loc="upper right")

    plt.show()

elif opcion == 5:
    puntaje_udec = udec(
        nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias
    )
    print(f"Puntaje ponderado en la Universidad de Concepción es: {puntaje_udec:.2f}")

    plt.figure(facecolor="#e9e0e0")
    plt.subplot(2, 1, 1)
    plt.bar(
        [
            "NEM",
            "Ranking",
            "CL",
            "M1",
            "M2",
            "Ciencias",
        ],
        [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias],
        color="blue",
    )
    plt.title("Puntajes PAES")
    plt.ylim(100, 1000)
    plt.tight_layout()

    plt.subplot(2, 1, 2)
    plt.bar(
        ["Puntaje ponderado", "Puntaje de corte"],
        [puntaje_udec, 804.75],
        color="blue",
        label=[f"Puntaje ponderado: {puntaje_udec:.2f}", "Puntaje de corte: 804.75"],
    )
    plt.title("Ingeniería Civil en Informática")
    plt.ylim(100, 1000)
    plt.tight_layout()
    plt.legend(loc="upper right")

    plt.show()

elif opcion == 6:
    puntaje_udp = udp(
        nem,
        ranking,
        competencia_lectora,
        matematicas_1,
        matematicas_2,
        ciencias,
        historia,
    )
    print(f"Puntaje ponderado en la Universidad Diego Portales es: {puntaje_udp:.2f}")

    if ciencias > historia:
        plt.figure(facecolor="#e9e0e0")
        plt.subplot(2, 1, 1)
        plt.bar(
            [
                "NEM",
                "Ranking",
                "CL",
                "M1",
                "M2",
                "Ciencias",
            ],
            [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, ciencias],
            color="blue",
        )
        plt.title("Puntajes PAES")
        plt.ylim(100, 1000)
        plt.tight_layout()
    else:
        plt.figure(facecolor="#e9e0e0")
        plt.subplot(2, 1, 1)
        plt.bar(
            [
                "NEM",
                "Ranking",
                "CL",
                "M1",
                "M2",
                "Historia",
            ],
            [nem, ranking, competencia_lectora, matematicas_1, matematicas_2, historia],
            color="blue",
        )
        plt.title("Puntajes PAES")
        plt.ylim(100, 1000)
        plt.tight_layout()

    plt.subplot(2, 1, 2)
    plt.bar(
        ["Puntaje ponderado", "Puntaje de corte"],
        [puntaje_udp, 748.7],
        color="blue",
        label=[f"Puntaje ponderado: {puntaje_udp:.2f}", "Puntaje de corte: 748.7"],
    )
    plt.title("Ingeniería Civil Informática")
    plt.ylim(100, 1000)
    plt.tight_layout()
    plt.legend(loc="upper right")

    plt.show()
