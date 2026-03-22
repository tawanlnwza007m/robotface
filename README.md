def sleep_frame(s, t):
    base_cy = 30
    breathe = int(round(1 * math.sin(2 * math.pi * t)))
    cy = base_cy + breathe

    gap = 56
    twitch = (0.72 < t < 0.76)

    if twitch:
        eyes_block(s, cy, w=28, h=10, r=5, gap=gap)
    else:
        eyes_block(s, cy, w=30, h=4, r=2, gap=gap)

frame_sleep = new_screen()
sleep_frame(frame_sleep, t=0.5)
frame_sleep
