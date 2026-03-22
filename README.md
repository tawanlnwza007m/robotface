def ack_frame(s, t):
    bounce = int(round(1 * math.sin(2 * math.pi * t)))
    cy = 30 - bounce
    smile_pointy_eyes(s, cy, gap=52, w=26, peak=10, thickness=3)

frame_ack = new_screen()
ack_frame(frame_ack, t=0.2)
frame_ack
