# data-analyst-test-task
1) 6 * (1 - (5/6)^6) ≈ 3.99
2) 26,83 для одного ((k - 1) / 79)^2
для всех сумма ((k - 1) / 79)^2 где к от 1 до 80
формула суммы квадратов n(n + 1)(2n + 1) / 6
(80*159/6)/79 ≈ 26,83
3) 0.63 за 10, 93.3 за 27
p(ни одной) = e^(-λt)
4)
def is_isomorphic(s, t):
    if len(s) != len(t):
        return False

    map_s_to_t = {}
    map_t_to_s = {}

    for char_s, char_t in zip(s,t):
        if char_s in map_s_to_t and map_s_to_t[char_s] != char_t:
            return False

        if char_t in map_t_to_s and map_t_to_s[char_t] != char_s:
            return False

        map_s_to_t[char_s] = char_t
        map_t_to_s[char_t] = char_s

    return True
