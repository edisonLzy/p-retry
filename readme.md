在指数回退策略中，参数的含义如下：

retries: 最大重试次数。
factor: 每次重试的时间间隔乘以该因子，用于计算下一次重试的时间间隔。例如，第一次重试等待1秒，第二次重试等待3秒，第三次重试等待9秒，以此类推。
minTimeout: 第一次重试的等待时间。
maxTimeout: 最大等待时间。如果重试时间超过此时间，则不再重试并返回错误。
randomize: 是否在计算下一次重试的时间间隔时添加随机因素，以避免所有重试都同时发生