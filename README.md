# J002 Vue+SpringBoot电影推荐可视化系统|双协同过滤推荐算法评论情感分析spark数据分析|配套文档1.34万字

> 完整项目收费，可联系QQ: 81040295 微信: mmdsj186011 注明从git来的，谢谢！
> 也可以关注我的B站： 麦麦大数据 https://space.bilibili.com/1583208775

关注B站，有好处！
编号:  J002
## 视频

[video(video-0FL1yxgl-1756613198617)(type-bilibili)(url-https://player.bilibili.com/player.html?aid=692406721)(image-https://i-blog.csdnimg.cn/img_convert/9fc75357c1dff4f800b8fd681ebb650e.jpeg)(title-spark+vue+springboot 电影大数据推荐情感分析bilstm 可视化协同过滤推荐算法系统源码全套)]

## 1 系统简介
本系统是一个基于Vue.js和Spring Boot技术栈构建的智能电影推荐可视化平台。系统采用前后端分离架构，通过三个不同的Vue前端界面（网站系统、管理系统、数据大屏）为用户、管理员和数据分析师提供差异化服务。系统集成了多种推荐算法（UserCF协同过滤、ItemCF推荐、LSTM情感分析等），结合MySQL数据库存储海量电影数据，为用户提供个性化电影推荐服务。同时，系统具备完善的数据可视化功能，支持电影评分统计、票房分析、用户行为分析等多维度数据展示，为电影行业决策提供数据支撑。
## 2 功能设计
系统采用经典的B/S架构模式，分为表现层、业务逻辑层和数据持久层。前端使用Vue.js框架配合Vue-router、ECharts等组件库构建响应式用户界面，后端基于Spring Boot框架提供RESTful API服务，使用MyBatis-Plus作为ORM框架简化数据库操作。系统核心推荐引擎集成了协同过滤算法和深度学习模型，通过分析用户历史行为和电影特征实现智能推荐。数据层采用MySQL关系型数据库确保数据一致性和可靠性。整体架构具有高内聚低耦合的特点，支持水平扩展，便于后期功能迭代和性能优化，为用户提供流畅的交互体验。

### 2.1系统架构图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/7ba661587d694dbeb8a77dc7120d2ee2.png)
### 2.2 功能模块图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c434d57771444bed92e4bba9ce862c28.png)
### 2.3 配套文档 1.34万字
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/ccab6ecd1d9c466a87ee76a22e533e4f.png)
### 2.4 项目目录
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/da2ffb437305463c8d1443c1111d1a08.png)
## 3 网站 功能展示
### 3.1 登录 & 注册
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/eedf752b7dfd463dabd46142ec8dcf5c.png)
### 3.2 主页 & 数据统计
提供网站的整体数据概览和统计信息，可能包括各种类型电影的数据统计等，让用户对网站运营状况有所了解。 【查看电影出品国和各种类型电影的统计】
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/04fe4e9e59dd452c84471e3c419ff280.png)
### 3.3 推荐算法
这是系统的核心功能之一。利用用户协同过滤 (UserCF) 和 物品协同过滤 (ItemCF) 算法为用户推荐电影。
- UserCF (基于用户的协同过滤): 根据与当前用户兴趣相似的其他用户的偏好来推荐电影。
- ItemCF (基于物品的协同过滤): 根据用户之前喜欢过的电影找到与其相似的其他电影进行推荐。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a68f080f9a5c466b9887abc85319d97f.png)
### 3.4 可视化分析
- 评论分析: 以图表等可视化方式展示电影评论的相关数据，如热门评论、评分等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9aaaac043f02423185df49fe96ce2c04.png)
- 电影出品分析: 可视化展示电影相关数据，如电影的出品国、类型分析等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5e40e7f25f8246dbb313af49a30b2a14.png)
- 电影地图分析：根据电影的出品国，通过世界地图的颜色形式可视化出来。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d2d3adcc1fe145cbb185ce6f583a2bd3.png)
### 3.5 词云分析
词云分析: 对歌曲歌词进行文本分析，生成词云图，直观展示歌词中高频出现的关键词，帮助用户快速了解歌曲主题或风格。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d5a0640b63224b6abef18f9cce78bde6.png)
### 3.6 修改密码
提供用户更改密码的功能。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f5d01177a7834b7b809643c7f700394f.png)
### 3.7 数据查询
允许用户根据关键词、电影、演员等条件查询电影信息。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a8deb387e24e413cac272c77225ca915.png)
### 3.8 电影详情 
通过评分控件可以进行电影评分
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8b776c34d9df4314a561caddbd286c3e.png)
评论通过LSTM进行情感分析，会给出情感分析的结果（好评 or 差评）
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/24ea8a8be14a4fbf8db782e65e6ca600.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/bdb7214eaa23476989aa8ccfafccad20.png)
## 4 管理系统 功能展示
### 4.1 登录 
该模块主要面向系统管理员，用于对网站内容、用户和数据进行管理和维护。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/38ef21d5f49647abb0ff2db2081c98be.png)
### 4.2 主页
查看目前系统运行情况的统计，还可以通过图形分析目前用户的来源【饼图】，以及用户性别【柱状图图】
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/49a85a87ab5f44fd9817dfb03a5c9b04.png)
### 4.3 管理个人信息
用户可以自行管理和修改个人资料，如昵称、头像、密码等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e9c07c7642c343869db5b54c2483d257.png)

### 4.4 权限
 对系统用的权限进行管理
 ![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/654b3ff8a26f4e20adc31d09fef23af7.png)

### 4.5 用户管理
对系统用户进行管理。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/310a74ab736b46129b04e8fb5b561203.png)
### 4.6 电影管理
 对电影信息进行管理，包括电影名称、类型、简介、评分、封面等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2cc0f5c9e5454459bc1de37972174e72.png)
### 4.7评论管理
管理用户对电影的评论，包括审核、删除违规评论等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/85381bd5eab54987aadef57f68779679.png)
## 5 可视化大屏 功能展示
### 5.1 数据大屏

评分分析、登录分析、评论分析、交互分析、登录分析、热门类型分析、评分分析、国产分析、词云分析等多维度数据可视化展示示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/43570f001bf4412bb5567d7a6ac56a52.png)
## 6 程序代码
### 6.1 代码说明
代码介绍：该Java协同过滤电影推荐系统基于用户行为数据实现个性化推荐。系统核心使用基于用户的协同过滤算法，通过余弦相似度计算用户之间的兴趣相似度。首先构建用户-歌曲评分矩阵存储播放数据，然后为每个用户计算Top-N相似用户群。推荐生成阶段，系统聚合相似用户看过但目标用户未接触的电影，根据相似度权重计算歌曲推荐得分，最后输出得分最高的电影作为推荐结果。算法采用内存数据结构存储关系，支持实时更新用户行为。系统包含关键模块：评分数据管理、相似度计算引擎、推荐生成器。通过调整相似用户数量和推荐条目数，可平衡推荐精度与计算效率，适合中等规模电影平台的推荐场景。
### 6.2 流程图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8824bc26607646e38314d21c595cc908.png)
### 6.3 代码实例
```java
import java.util.*;

public class MovieRecommender {
    // 用户-电影评分矩阵 (用户ID -> (电影ID -> 评分))
    private Map<Integer, Map<Integer, Double>> userMovieRatings;

    public MovieRecommender() {
        userMovieRatings = new HashMap<>();
    }

    // 添加用户评分
    public void addRating(int userId, int movieId, double rating) {
        userMovieRatings.computeIfAbsent(userId, k -> new HashMap<>()).put(movieId, rating);
    }

    // 计算余弦相似度
    private double cosineSimilarity(Map<Integer, Double> user1, Map<Integer, Double> user2) {
        double dotProduct = 0.0;
        double norm1 = 0.0;
        double norm2 = 0.0;

        // 遍历用户1评分的电影
        for (Map.Entry<Integer, Double> entry : user1.entrySet()) {
            int movieId = entry.getKey();
            double rating1 = entry.getValue();
            
            // 如果用户2也评分了该电影
            if (user2.containsKey(movieId)) {
                double rating2 = user2.get(movieId);
                dotProduct += rating1 * rating2;
            }
            norm1 += Math.pow(rating1, 2);
        }

        // 计算用户2的范数
        for (double rating : user2.values()) {
            norm2 += Math.pow(rating, 2);
        }

        if (norm1 == 0 || norm2 == 0) return 0;
        return dotProduct / (Math.sqrt(norm1) * Math.sqrt(norm2));
    }

    // 获取最相似的用户
    private List<Integer> getSimilarUsers(int targetUserId, int topN) {
        Map<Integer, Double> targetUser = userMovieRatings.getOrDefault(targetUserId, new HashMap<>());
        PriorityQueue<Map.Entry<Integer, Double>> pq = new PriorityQueue<>(
            (a, b) -> Double.compare(b.getValue(), a.getValue())
        );

        for (int userId : userMovieRatings.keySet()) {
            if (userId == targetUserId) continue;
            double similarity = cosineSimilarity(targetUser, userMovieRatings.get(userId));
            pq.offer(new AbstractMap.SimpleEntry<>(userId, similarity));
        }

        List<Integer> similarUsers = new ArrayList<>();
        for (int i = 0; i < topN && !pq.isEmpty(); i++) {
            similarUsers.add(pq.poll().getKey());
        }
        return similarUsers;
    }

    // 生成电影推荐
    public List<Integer> recommendMovies(int targetUserId, int numRecommendations) {
        Map<Integer, Double> targetUser = userMovieRatings.get(targetUserId);
        List<Integer> similarUsers = getSimilarUsers(targetUserId, 5);
        Map<Integer, Double> movieScores = new HashMap<>();

        // 计算未观看电影的推荐分数
        for (int userId : similarUsers) {
            Map<Integer, Double> ratings = userMovieRatings.get(userId);
            for (Map.Entry<Integer, Double> entry : ratings.entrySet()) {
                int movieId = entry.getKey();
                double rating = entry.getValue();
                
                // 跳过目标用户已经看过的电影
                if (targetUser.containsKey(movieId)) continue;
                
                // 加权求和：相似度 * 评分
                movieScores.put(movieId, movieScores.getOrDefault(movieId, 0.0) + rating);
            }
        }

        // 按推荐分数排序
        PriorityQueue<Map.Entry<Integer, Double>> pq = new PriorityQueue<>(
            (a, b) -> Double.compare(b.getValue(), a.getValue())
        );
        pq.addAll(movieScores.entrySet());

        // 返回前N个推荐
        List<Integer> recommendations = new ArrayList<>();
        for (int i = 0; i < numRecommendations && !pq.isEmpty(); i++) {
            recommendations.add(pq.poll().getKey());
        }
        return recommendations;
    }

    // 测试用例
    public static void main(String[] args) {
        MovieRecommender recommender = new MovieRecommender();
        
        // 添加样本数据
        recommender.addRating(1, 101, 4.5);
        recommender.addRating(1, 102, 3.0);
        recommender.addRating(2, 101, 4.0);
        recommender.addRating(2, 103, 5.0);
        recommender.addRating(3, 102, 2.5);
        recommender.addRating(3, 103, 4.5);
        recommender.addRating(3, 104, 3.5);

        // 为用户1生成推荐
        List<Integer> recommendations = recommender.recommendMovies(1, 2);
        System.out.println("为用户1推荐的电影: " + recommendations);
    }
}

```
